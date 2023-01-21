An _association_ is a connection between two Active Record models.

Rails support six types of assciations
- `belongs_to`
- `has_one`
- `has_many`
- `has_many :through`
- `has_one :through`
- `has_and_belongs_to_many`

### Create One to Many Relation

#### Student - Blogs (One Student Many Blogs)

Student can have many blogs so in blogs Model use `belongs to: student`
In the blogs model we need to create a `student_id` first which will serve as foreign key
```rb
class CreateBlogs < ActiveRecord::Migration[7.0]
  def change
    create_table :blogs do |t|
      t.string :title
      t.text :content
      t.integer :student_id

      t.timestamps
    end
  end
end

```

```rb
class Blog < ApplicationRecord
	belongs_to :student
end
```

In student model use `has_many: blogs`
```rb
class Student < ApplicationRecord
	has_many :blogs
end
```
##### Operations 

- To Create a new blog:
```rb
stu = Student.new do |s|
		s.name = "Kushal"
		s.email = "kushal@gmail.com"
	end

stu.blogs.create(title: "New Generations", content: "This is content of blog" )

```

- To get all blogs of a student : 
```rb
stu = Student.find(1)
stu.blogs
```

#### Summary
1. Create a User Model
2. Create a Blogs Model
3. Add `user_id` column in **Blogs Migration**
4. Add `has_many :blogs` in **Student Model**
5. Add `belongs_to :student` in **Blogs Model**


### Create Many to Many Relation
There are two ways to create many to many relations

#### 1. has_and_belongs_to_many

- `has_and_belongs_to_many` - Creates many to many relationships
- It do not require any interveing model
- But it require to create a **join table** 

##### Steps
1. Create A **Student Model** and **Course Model**
2. In the Student and Course Model add `has_and_belongs_to_many`

**StudentModel** `models/student.rb`
```rb
class Student < ApplicationRecord
    has_many :blogs 
    has_and_belongs_to_many :courses
end
```

**CourseModel** `models/course.rb`
```rb
class Course < ApplicationRecord
    has_and_belongs_to_many :students
end
```

3. Create a migration for join table.
```rb
class CreateCourseStudentJoinTable < ActiveRecord::Migration[7.0]
  def change
    create_join_table :courses, :students 
  end
end
```

4. Run the migration to add this table in our schema. `rails db:migrate`
5. Now we have created many to many relation between Students and Course.

##### Operations
```rb
stu = Student.create(name: "Kushal", email: "kushal@gmail.com", age: 22)

# TO create a course
stu.courses.create(name: "Web Development", description: "Website Development", points: 40)

# Same can be done by course to student.
```

#### Summary
1. Create a student and course model and migrate them too.
2. Add `has_and_belongs_to_many : students/courses` in both the model file.
3. Now create a join table `create_join_table :courses, :students`.
4. Now we have successfully created many to many relationship.

#### 2. has_many: through
