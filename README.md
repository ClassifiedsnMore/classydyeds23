# classydyeds23
classifieds for personal sex wants
how to enjoy yourself discrettly







File.fnmatch('cat',       'cat')        #=> true  # match entire string
File.fnmatch('cat',       'category')   #=> false # only match partial string

File.fnmatch('c{at,ub}s', 'cats')                    #=> false # { } isn't supported by default
File.fnmatch('c{at,ub}s', 'cats', File::FNM_EXTGLOB) #=> true  # { } is supported on FNM_EXTGLOB

File.fnmatch('c?t',     'cat')          #=> true  # '?' match only 1 character
File.fnmatch('c??t',    'cat')          #=> false # ditto
File.fnmatch('c*',      'cats')         #=> true  # '*' match 0 or more characters
File.fnmatch('c*t',     'c/a/b/t')      #=> true  # ditto
File.fnmatch('ca[a-z]', 'cat')          #=> true  # inclusive bracket expression
File.fnmatch('ca[^t]',  'cat')          #=> false # exclusive bracket expression ('^' or '!')

File.fnmatch('cat', 'CAT')                     #=> false # case sensitive
File.fnmatch('cat', 'CAT', File::FNM_CASEFOLD) #=> true  # case insensitive

