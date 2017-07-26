# Ruby Questions

## Which of the expressions listed below will result in "false"?
```ruby
true    ? "true" : "false"
false   ? "true" : "false"
nil     ? "true" : "false"
1       ? "true" : "false"
0       ? "true" : "false"
"false" ? "true" : "false"
""      ? "true" : "false"
[]      ? "true" : "false"
```

### Answer
```ruby
false   ? "true" : "false"
nil     ? "true" : "false"
```

## I want to write some code that takes an array of numbers, multiplies each item in the array by 3, and returns a new array with the new values. know I should use #map, #each, or #select, but I’m not sure which one is best -- teach me.

### Answer
>You could do using either #map or #each, however using #map will be more efficient since it will automatically return the modified array after applying your block on it whereas each will just apply the logic to each element and you would have to store this in a new array and then return that array.  #Map already automatically runs #each on the array and then returns the result.  #Select does something entirely different as it will run the block on each element and then return an array of elements that passed as "true" on the block.  Here's how the code would look:

```ruby
arr.map {|x| x * 3}
```

## What are the common controller actions?

### Answer
>The common Rails controller actions (CRUD) are index, show, new, create, edit, update, and destroy.

## Which of the following is not a benefit of Object-Oriented Programming?

a) Reduces side effects of functions
b) Enables code reuse
c) Encapsulates functionality
d) Allows the developer to make certain methods/variables inaccessible to other classes

### Answer
>a) Reduces side effects of functions

## Consider the following two methods:
```ruby
def times_two(arg1);
  puts arg1 * 2;
end

def sum(arg1, arg2);
  puts arg1 + arg2;
end
```
What will be the result of each of the following lines of code:
```ruby
times_two 5
times_two(5)
times_two (5)
sum 1, 2
sum(1, 2)
sum (1, 2)
```

### Answer
```ruby
$ times_two 5
> 10

$ times_two(5)
> 10

$ times_two (5)
> 10

$ sum 1, 2
> 3

$ sum(1, 2)
> 3

$ sum (1, 2)
> error
```

## What is missing? M_____/View/Controller

### Answer
>Model

## What is the most beneficial aspect of TDD?

### Answer
>You gain the ability to refactor and extend code without fear of breaking the application in unexpected ways since each piece of logic and functionality is tested.  You also gain the benefit of never-ending frustration as you constantly have to break the "coding cycle" to go write tests first (lol).

## Write a function that accepts an array of numbers and a second number. Beginning at index 0, total up the sum of the values of the array until you've met or surpassed the second argument. Return the number of elements required to fulfill the goal. If the goal can't be reached, return 0.

### Answer
```ruby
def foo(arr, bar)
  sum = 0
  sol = 0
  while sum < bar
    sum += arr[sol]
    sol += 1
    return 0 if sol >= arr.length
  end
  sol
end
```

## Make a copy of http://jsbin.com/beyape/1/edit complete the task described in the comments and attach the link

### Answer
>Ok, I had to look some stuff up on this one.  It started coming back quickly, but yea, a lot of the basics on JS and jQuery are faded in my mind since I've been working with ruby so long.  Any chance you could send me a couple more exercises just to help jog my memory a bit more before the assessment?  In any case, here's the link: http://jsbin.com/garizasalu/edit?html,js,output