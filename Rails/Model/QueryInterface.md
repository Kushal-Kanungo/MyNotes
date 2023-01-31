#### 1. find 
**find** : we can find retrieve an object from database by passing the **primary key**.
```rb
# To find a user with id 1
user = User.find(1)

# To find users present in the array
users = User.find([1,2,3,4,5])

```
> **Note:** It will raise an `ActiveRecord::RecordNotFound` error 
---

#### 2. take
**take** : It retrives **one or more records** in no implicit ordering
```rb

user = User.take(1) # retrive one record from the table 

user = User.take(5) #Select * from user LIMIT 5

```
> **NOTE** : It will return *nil* if no record found.

**take!** : will raise error if record not found

---

#### 3. first / last
**first** : retrieve **first record** order by primary key ascending
**last** : retrive **first record** order by primary key desceneding

`first!` and `last!` will raise an error if record not find

---

#### 4. find_by
We can find a **single record** by specifing the attribute name.
```rb
user = User.find_by(name: "Kushal")

#Same as
user = User.where(name: "Kushal").take!

```


## Retrieving Multiple Objects
```rb
# This may consume too much memory if the table is big.
Customer.all.each do |customer|
  NewsMailer.weekly(customer).deliver_now
end

```

To retrive in batches we have.

#### 5. find_each
It retrives the records on **batches** and then yields each one in block.
```rb
Customer.find_each do |customer|
  NewsMailer.weekly(customer).deliver_now
end
```

##### batch_size
We can pass batch size using `batch_size: 5000`
```rb
Customer.find_each(batch_size: 5000) do |customer|
  NewsMailer.weekly(customer).deliver_now
end
```

##### start / finish
We can define **starting point** from where we want to find records and **ending point**.
```rb
Customer.find_each(start: 2000, finish:9000) do |customer|
  NewsMailer.weekly(customer).deliver_now
end
```

---

#### 6. find_in_batches
Same as find_each but it yields block as an array upto 1000 records at a time
```rb
# Give add_customers an array of 1000 customers at a time.
Customer.find_in_batches do |customers|
  export.add_customers(customers)
end
```

##### Some options we can pass
**:batch_size**, **:start**, **:finish**

