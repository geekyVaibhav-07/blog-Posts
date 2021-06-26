# blog-posts
Posts service for project blog

Services: 
    - get post/posts
    - create a new post
    - update post
    - delete post

Routes: 
    - path : /posts
    - methods:
        - get: get post/posts
        - post: create a new post
        - put: updated a post
        - delete: delete a post

Schema of a post: 
    {
        id: ObjectId
        title: String
        createdBy: String | UserId
        Content: String
        createdOn: DateTime
        updatedOn: dateTime
        category: String
        subCategory: String
        primaryImage: String
        attachedImages: List
        references: List
    }