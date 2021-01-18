# Mongify ChangeLog

## 1.3.2 / 04 Sep 2017
* Minor code refactoring
* Removed exception handling around ALL exceptions (this should improve finding issues outside of Mongify)

## 1.3.1 / 09 Nov 2016
* Updated gem requirements to exlucde ActiveRecord/ActiveSupport 5.0
* Locked down gem versions to prevent issues on newer gems (Like ActiveRecord 5 and Mongo)
* Updated README with better markdown
* Updated 'add_dependency' to 'add_runtime_dependency' in gemspec
* Updated some development gems

## 1.3.0 / 07 May 2016
* Updated gem requirements to ActiveRecord 4.2
* Updated type casting to ActiveRecord 4.2 style.
  * NOTE: Timezone is set to UTC by default in the database
* Removed tons of deprication warnings during tests
* Improved contribution set-up rake tasks
* Included Postgres config for Contributors (NOTE: No tests for this)
* Ensured updated_at doesn't get parsed multiple times in `sync` command (thanks @hammady)
* Improved error message during `sync` command (thanks @hammady)
* Minor bug fixes
## 1.2.4 / 29 July 2014
* 
* Moved the order of reference updating to be second (after copying tables), this way embed tables can use new references
* Small tweak on table.name (making sure rename_to value gets returns first) - It wasn't commited in version 1.2.3
## 1.2.3 / 17 July 2014
* Fixed MS Sql batching issue
* Fixed row.delete requiring you to send in a string (vs symbol)
* ~~Small tweak on table.name (making sure rename_to value gets returns first)~~
## 1.2.2 / 9 July 2014
* Locked in BSON and rspec gem to versions that will work with Mongify
* Updated gems
## 1.2.1 / 16 June 2014
* Fixed polymorphic associations not getting set properly
## 1.2 / 16 June 2014
* Added batching to embedded and polymorphic tables.
* Tweaked progress bar display.
* Fixed issue with embedding
* Updated mongo drivers to version 1.10.2
