---
layout: post
title:      "On Data Structures in Ruby"
date:       2018-11-10 14:54:11 -0500
permalink:  on_data_structures_in_ruby
---


What are data structures and why are they so important?  Data structures achieve the critical task of storing information and giving structure to data.  Data structures make our programming lives so much easier, so let's see what all the hubhub is about.

The first and simplest data structure we will discuss is the array.  An array is a collection of ordered data with an integer index.  The following is an example of an array:   

array = ["Mike", "Steve", "Tim"]

array[0]  # => "Mike"
array[1]  # => "Steve"
array[2]  # => "Tim"   

We can see that our data, the three names, is ordered with an integer index.  It is important to remember that every array starts with an index of 0.  Thus,  "Mike" is located at index 0, "Steve is located at index 1, and "Tim" is located at index 2.  A negative index will reference the end of an array.

array[-1]  # => "Tim"
array[-2]  # => "Steve"
array[-3]  # => "Tim"

There are built-in Ruby methods that allow us to manipulate arrays and the data contained therein.  For example, if we want to add elements to an array, we can use the push method.  If we want to add "John" to the end of the array, we can do so using the push method.

array.push("John")  # => ["Mike", "Steve", "Tim", "John"]

We can also create arrays that contain one or more arrays inside the original array.  These are called nested array.  The following is an example of a simple nested array.

example_array = ["university", ["biology", "math", "history]]

If we want to retrieve the array nested within example_array, we simply access the data as if it were any other element in an array by using its integer index, which in this case is 1.

example[1] # => ["biology", "math", "history]

To access "history" in the nested array, we would write the following code using the integer index for "history", which in this case is 2.
```
example[1][2] # => "history"

In addition to the array, another very commonly used data structure is the hash.  A hash is a collection of data organized by key-value pairs.  Unlike the array that uses an integer index, the hash uses keys as the indices of the hash and they can be of any object type, ie. string, integer, etc.  The following is an example of a hash:

hash={"testscore" => 89, "school" => "NYU"}

The keys in the hash are the strings "testscore" and "school" and we use them to access the values they contain in the hash.

hash["testscore"]  # => 89
hash["school"]  # => "NYU"

Notice that this retrieval method is identical to that in an array except we use the key instead of an integer to retrieve the value we are looking for.  Also, each value in the hash must have a unique key which again is identical to an array in which each element has a unique integer index.

Ruby also has built-in methods that allow us to work with and manipulate hashes.  For example, if we want to retrieve all the keys in a hash, we can use the keys method which will return an array containing the keys of the hash.  Calling the method keys on the above hash will return ["testscore","school"].

hash.keys  # => ["testscore","school"]

Just as we can create nest arrays, we can also create nested hashes.  The following is an example of a nested hash.

example_hash = {"nachos" => {"snack_type" =>"chips", "flavoring" => "spicey"}}

To retrieve the inner hash, we would use the key "nachos"  to retrieve the hash.  Thus, example_hash["nachos"] will return {"snack_type" =>"chips", "flavoring" => "spicey"}.

example_hash["nachos"]  # =>  {"snack_type" =>"chips", "flavoring" => "spicey"}  

If we want to retrieve the data from within the inner, nested hash itself, we first use the outer, top level key followed by the inner, lower level key, to pull that information out.  In this example, we use the key "nachos" followed by the key "snack_type" to retrieve the value "chips".

example_hash["nachos"]["snack_type"] # => "chips"  

Nested hashes can also contain arrays.  We can change our example_hash to include an array.

example_hash["nachos"]  =>  {"snack_type" =>"chips", "flavoring" => ["spicey", "hot"]} 

To access the data in the array in the nested hash, we use the key "nachos" followed by the key "snack_type" followed by the index 0 to retrieve "spicey".

example_hash["nachos"]["snack_type"][0]  # => "spicey"

The possibilities of arranging data are virtually limitless using data structures such as arrays and hashes.  The more complex the data and data associations that we as programmers work with,  the more complex we can correspondingly make our data structures.  The hub hub about data structures is simply the flexibility and power that we as programmers can access for whatever information we are dealing with when working on a program.













































