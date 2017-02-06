v# Lesson 1
## **Creating a new Rails application**
```Bash
$ rails new XXXXXX
```

## **Making new Controller and Action**
```Bash
$ rails generate controller xxx yyy
```

## **Setting routes**
* Copying _config/routes.rb_ 

* Modifying [_config/application.rb_](testtwitter/config/application.rb) file  
```Code
config.sass.preferred_syntax = :sass
```

## **install authentication library**
* Installing sorcery
```Bash
$ rails g sorcery:install
```

## **Created Model and View**
* Creating **Model** (_users_) and **View**
```Bash
$ rails g scaffold user -s --no-stylesheets --skip-migration
```

* Creating add data(_name_ and _screen name_ and _bio_) to **Users Model**
```Bash
$ rails g migration add_name_and_screen_name_and_bio_to_users name:string screen_name:string bio:string
```

* Mounting database
```Bash
$ rake db:migrate
```

## **Created Registration function**
* Creating registrations controller
```Bash
$ rails generate controller registrations new
```

## **Modify Layout**
* Modify [_app/views/layouts/application.html.erb_](testtwitter/app/views/layouts/application.html.erb) file  
* Let's Check Web Page

## **Setting Route**
* Copying [_routes.rb_](testtwitter/config/routes.rb) file to _config_ folder  
* Let's Check Web Page

## **Making Registration Screen**
* Implementing _User_ Model  
Modify [_app/models/user.rb_](testtwitter/app/models/user.rb) file.  
Using _Validation_.
* Implementing _Registration_ Controller  
 Modify [_app/controllers/registrations\_controller.rb_](testtwitter/app/controllers/registrations_controller.rb) file.
* Implementing _New_ View  
Modify [_app/views/registrations/new.html.haml_](testtwitter/app/views/registrations/new.html.haml) file.  
* Let's Check Web Page  
