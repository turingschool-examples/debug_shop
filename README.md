# Debug Shop

## What is this?
Debug Shop is a repo with a lot of bugs in it... your goal is to find and fix them all! For each failing test, read error messages, pry through your Rails app, and get each test to pass.

## Learning Goals
* Utilize pry in Rails
* Understand and Interpret Error/Failure messaages

### Setup

* Clone this repo to your local computer
* Run `bundle install`
* Run `rake db:{create,migrate}` (note: this will set off your first error)

### Exercise Instructions

* As stated above, your first error that you'll have to fix will come up when you try to migrate. Fix this first.
* After fixing the above error, run and fix the following tests in this specific order:
  Model Tests:
    - `rspec spec/models/merchant_spec.rb`
    - `rspec spec/models/item_spec.rb`
    - `rspec spec/models` (to confirm that all model tests are now passing)

  Feature Tests:
    - `rspec spec/features/merchants/index_spec.rb`
    - `rspec spec/features/merchants/show_spec.rb`
    - `rspec spec/features/merchants/new_spec.rb`
    - `rspec spec/features/merchants/edit_spec.rb`
    - `rspec spec/features/merchants/destroy_spec.rb`
    - `rspec spec/features/items/index_spec.rb`
    - `rspec spec/features/items/merchant_items_index_spec.rb`
    - `rspec spec/features/items/new_spec.rb`
    - `rspec spec/features/items/edit_spec.rb`
    - `rspec spec/features/items/show_spec.rb`
    - `rspec spec/features` (to confirm that all feature tests are now passing)
