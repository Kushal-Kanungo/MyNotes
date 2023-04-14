	
### Using includes
```rb
user = User.includes(:posts).select("users.*, posts.id, posts.title").find(params[:id])
```


### Using preload
```rb
users = User.preload(posts: [:id, :title], comments: [:id, :body])

users.each do |user|
  puts "User #{user.id} has #{user.posts.size} posts and #{user.comments.size} comments"
end

```
