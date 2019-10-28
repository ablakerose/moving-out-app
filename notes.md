Moving Out

User
- has_many :items
name
status (buyer/seller)

Item
- belongs_to :user
- has_many users, through :offers
name



Offer
has_many :users
has_many :items

For join table, think about how we want our relationships to interact with each other. A join table should only happen when we have a many to many relationship, to ensure there is a purpose for it. 