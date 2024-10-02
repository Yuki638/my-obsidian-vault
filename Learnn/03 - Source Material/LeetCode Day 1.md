just gunna select what im going to work with

<font color="red">Given an array of integers `nums` and an integer `target`, return _indices of the two numbers such that they add up to `target`_.

You may assume that each input would have **_exactly_ one solution**, and you may not use the _same_ element twice.

You can return the answer in any order.</font>

I have to learn indices 

not really because there are some examples

**Example 1:**

**Input:** nums = [2,7,11,15], target = 9
**Output:** [0,1]
**Explanation:** Because nums[0] + nums[1] == 9, we return [0, 1].

**Example 2:**

**Input:** nums = [3,2,4], target = 6
**Output:** [1,2]

**Example 3:**

**Input:** nums = [3,3], target = 6
**Output:** [0,1]


a prototype that will go with every elements in the array and try to sum between two or more elements in the array to find a target set by the user for example we have an array [1,2,3,4] and the user sets the target as 5 then the result or outcome will be a list saying the index of the numbers whose sum is the resulting target value in this case we get a output like [0,3]

for this operation we'd need [[numpy]] for sure to make and create array efficiently then we also need to find out a way by which we can initiate the sum of every and each elements of the array let's see if theres some prebuilt function in the module or not or we have to make a one that satisfies our problem 