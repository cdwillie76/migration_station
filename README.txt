= migration_station

== DESCRIPTION:

All aboard!  Do you love the way Rails handles migrations?  Do you have non-Rails projects that could benefit from migrations?  Well set yourself up a migration station and get to work! 


== PROPOSED MIGRATION GENERATORS:
* table_migration - This migration will [eventually] generate the same 
style migrations that are generated when creating a Rails model.  Proposed 
syntax: script/generate table_migration Users first_name:text 
last_name:text to generate the up and down migration methods filled with 
the appropriate information from the arguments.

* migration - This generates a standard migration.  If possible (this is 
where help will come in handy!), establish the Rails style 
"script/generate migration AddAgeToUsers" to generate the 
migration with the up and down migration methods adding and removing the 
column from the table stated in the argument.


== PROPOSED USAGE

migration_station ProjectName
cd ProjectName
.script/generate table_migration User first_name:text last_name:text
.script/generate migration AddAgeToUser
rake migrate

== LICENSE:

(The MIT License)

Copyright (c) 2008 Matthew Williams

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
