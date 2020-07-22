# LEETCODE API

## Overview

I made this API for my discord bot but I am making this project public. Please email ashishsushilpatel@gmail.com if you find any bugs.

## Routes

URL | Description
------|------------
**https://leetcode.ashish.me/api/problem | Returns a random leetcode problem
https://leetcode.ashish.me/api/problem?difficulty=1 | Returns a random leetcode problem with difficulty filter (1=easy, 2=medium, 3=hard)
https://leetcode.ashish.me/api/problem?id=15| Returns leetcode question number 15 

## Examples

difficulty filter example: https://leetcode.ashish.me/api/problem?difficulty=1

```javascript
{
code: 200,
message: "Success",
response: [
{
id: 1022,
title: "Sum of Root To Leaf Binary Numbers",
slug: "sum-of-root-to-leaf-binary-numbers",
difficulty: 1,
question_no: 1022,
is_paid: 0,
url: "https://leetcode.com/problems/sum-of-root-to-leaf-binary-numbers",
content: "<p>Given a binary tree, each node has value <code>0</code>&nbsp;or <code>1</code>.&nbsp; Each root-to-leaf path represents a binary number starting with the most significant bit.&nbsp; For example, if the path is <code>0 -&gt; 1 -&gt; 1 -&gt; 0 -&gt; 1</code>, then this could represent <code>01101</code> in binary, which is <code>13</code>.</p> <p>For all leaves in the tree, consider the numbers represented by the path&nbsp;from the root to that leaf.</p> <p>Return the sum of thesenumbers.</p> <p>&nbsp;</p> <p><strong>Example 1:</strong></p> <p><span id="example-output-1"><img alt="" src="https://assets.leetcode.com/uploads/2019/04/04/sum-of-root-to-leaf-binary-numbers.png" style="width: 304px; height: 200px;" /></span></p> <pre> <strong>Input: </strong><span id="example-input-1-1">[1,0,1,0,1,0,1]</span> <strong>Output: </strong><span id="example-output-1">22</span> <strong>Explanation: </strong>(100) + (101) + (110) + (111) = 4 + 5 + 6 + 7 = 22 </pre> <p>&nbsp;</p> <p><strong>Note:</strong></p> <ol> <li>The number of nodes in the tree is between <code>1</code> and <code>1000</code>.</li> <li>node.val is <code>0</code> or <code>1</code>.</li> <li>The answer will not exceed <code>2^31 - 1</code>.</li> </ol> ",
solution: null,
likes: 517,
dislikes: 70,
sample_testcase: "[1,0,1,0,1,0,1]",
hints: [
"Find each path, then transform that path to an integer in base 10."
],
code_snippets: [
{
code: "/** * Definition for a binary tree node. * struct TreeNode { * int val; * TreeNode *left; * TreeNode *right; * TreeNode() : val(0), left(nullptr), right(nullptr) {} * TreeNode(int x) : val(x), left(nullptr), right(nullptr) {} * TreeNode(int x, TreeNode *left, TreeNode *right) : val(x), left(left), right(right) {} * }; */ class Solution { public: int sumRootToLeaf(TreeNode* root) { } };",
lang: "C++"
},
{
code: "/** * Definition for a binary tree node. * public class TreeNode { * int val; * TreeNode left; * TreeNode right; * TreeNode() {} * TreeNode(int val) { this.val = val; } * TreeNode(int val, TreeNode left, TreeNode right) { * this.val = val; * this.left = left; * this.right = right; * } * } */ class Solution { public int sumRootToLeaf(TreeNode root) { } }",
lang: "Java"
},
{
code: "# Definition for a binary tree node. # class TreeNode(object): # def __init__(self, val=0, left=None, right=None): # self.val = val # self.left = left # self.right = right class Solution(object): def sumRootToLeaf(self, root): """ :type root: TreeNode :rtype: int """ ",
lang: "Python"
},
{
code: "# Definition for a binary tree node. # class TreeNode: # def __init__(self, val=0, left=None, right=None): # self.val = val # self.left = left # self.right = right class Solution: def sumRootToLeaf(self, root: TreeNode) -> int: ",
lang: "Python3"
},
{
code: "/** * Definition for a binary tree node. * struct TreeNode { * int val; * struct TreeNode *left; * struct TreeNode *right; * }; */ int sumRootToLeaf(struct TreeNode* root){ }",
lang: "C"
},
{
code: "/** * Definition for a binary tree node. * public class TreeNode { * public int val; * public TreeNode left; * public TreeNode right; * public TreeNode(int val=0, TreeNode left=null, TreeNode right=null) { * this.val = val; * this.left = left; * this.right = right; * } * } */ public class Solution { public int SumRootToLeaf(TreeNode root) { } }",
lang: "C#"
},
{
code: "/** * Definition for a binary tree node. * function TreeNode(val, left, right) { * this.val = (val===undefined ? 0 : val) * this.left = (left===undefined ? null : left) * this.right = (right===undefined ? null : right) * } */ /** * @param {TreeNode} root * @return {number} */ var sumRootToLeaf = function(root) { };",
lang: "JavaScript"
},
{
code: "# Definition for a binary tree node. # class TreeNode # attr_accessor :val, :left, :right # def initialize(val = 0, left = nil, right = nil) # @val = val # @left = left # @right = right # end # end # @param {TreeNode} root # @return {Integer} def sum_root_to_leaf(root) end",
lang: "Ruby"
},
{
code: "/** * Definition for a binary tree node. * public class TreeNode { * public var val: Int * public var left: TreeNode? * public var right: TreeNode? * public init() { self.val = 0; self.left = nil; self.right = nil; } * public init(_ val: Int) { self.val = val; self.left = nil; self.right = nil; } * public init(_ val: Int, _ left: TreeNode?, _ right: TreeNode?) { * self.val = val * self.left = left * self.right = right * } * } */ class Solution { func sumRootToLeaf(_ root: TreeNode?) -> Int { } }",
lang: "Swift"
},
{
code: "/** * Definition for a binary tree node. * type TreeNode struct { * Val int * Left *TreeNode * Right *TreeNode * } */ func sumRootToLeaf(root *TreeNode) int { }",
lang: "Go"
},
{
code: "/** * Definition for a binary tree node. * class TreeNode(_value: Int = 0, _left: TreeNode = null, _right: TreeNode = null) { * var value: Int = _value * var left: TreeNode = _left * var right: TreeNode = _right * } */ object Solution { def sumRootToLeaf(root: TreeNode): Int = { } }",
lang: "Scala"
},
{
code: "/** * Example: * var ti = TreeNode(5) * var v = ti.`val` * Definition for a binary tree node. * class TreeNode(var `val`: Int) { * var left: TreeNode? = null * var right: TreeNode? = null * } */ class Solution { fun sumRootToLeaf(root: TreeNode?): Int { } }",
lang: "Kotlin"
},
{
code: "// Definition for a binary tree node. // #[derive(Debug, PartialEq, Eq)] // pub struct TreeNode { // pub val: i32, // pub left: Option<Rc<RefCell<TreeNode>>>, // pub right: Option<Rc<RefCell<TreeNode>>>, // } // // impl TreeNode { // #[inline] // pub fn new(val: i32) -> Self { // TreeNode { // val, // left: None, // right: None // } // } // } use std::rc::Rc; use std::cell::RefCell; impl Solution { pub fn sum_root_to_leaf(root: Option<Rc<RefCell<TreeNode>>>) -> i32 { } }",
lang: "Rust"
},
{
code: "/** * Definition for a binary tree node. * class TreeNode { * public $val = null; * public $left = null; * public $right = null; * function __construct($val = 0, $left = null, $right = null) { * $this->val = $val; * $this->left = $left; * $this->right = $right; * } * } */ class Solution { /** * @param TreeNode $root * @return Integer */ function sumRootToLeaf($root) { } }",
lang: "PHP"
},
{
code: "/** * Definition for a binary tree node. * class TreeNode { * val: number * left: TreeNode | null * right: TreeNode | null * constructor(val?: number, left?: TreeNode | null, right?: TreeNode | null) { * this.val = (val===undefined ? 0 : val) * this.left = (left===undefined ? null : left) * this.right = (right===undefined ? null : right) * } * } */ function sumRootToLeaf(root: TreeNode | null): number { };",
lang: "TypeScript"
}
],
topics: [
{
name: "Tree",
slug: "tree"
}
],
category: "Algorithms"
}
]
} 
```
