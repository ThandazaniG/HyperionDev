## Markdown file

## anagram.py

class Solution:
  def groupAnagrams(self, strs):
      result = {}
      for i in strs:
""" Line 5: the sorted() function expects an argument but 0 arguments were given, see variable i included """
          x = "".join(sorted(i))
          if x in result:
              result[x].append(i)
          else:
              result[x] = [i]
      return list(result.values())
""" The function call returns the expected output, pay careful attention to detail"""
ob1 = Solution()
print(ob1.groupAnagrams(["eat", "tea", "tan", "ate", "nat", "bat"]))
