lib: https://cplusplus.com/reference

数据库内核杂谈: https://www.infoq.cn/article/0rSVq2VIfUE0YLedLe5o


``` c++
#include<iostream>
#include<string>
#include<vector>
#include<unordered_set>
#include<unordered_map>

using std::cout;
using std::endl;
using std::string
using std::vector;
using std::unordered_set;
using std::unordered_map;
```

string
```c++
#include<string>
using string;

string s;

// 长度
auto s_len = s.length();

// 排序, 不会生成新变量, sort 可以直接用
sort(s.begin(), s.end());

// 
```

vector
```c++

// 初始化
vector<int> vec;
vector<int> vec_2(vec);
vector<int> nums = {4, 9, 5};
vector<int> nums{1, 3, 5};
vector<int> res(res_set.begin(), res_set.end());

// 7个0 和 7个3
vector<int> vec(7);
vector<int> vec(7, 3);

vector.push_back(item);

for(int i = 0; i < nums.size(); i++)
{
    
}

for(auto item : nums)
{
    cout << item << " ";
}

return {};
return vector<int>{1, 4}
return vector<int>(res_set.begin(), res_set.end());
```

unordered_set
```c++
#include<unordered_set>
using unordered_set;

// 初始化 num 是 vector<int>
unordered_set<int> nums_set(nums.begin(), nums.end());
unordered_set<int> res_set;

// 查找 插入: find 返回的是迭代器
nums_set.find(item) != nums_set.end();
res_set.insert(item);

// 在容器中搜索值为k的元素并返回找到的元素数。由于unordered_set容器不允许重复值，这意味着如果容器中存在具有该值的元素，则该函数实际上返回1 ，否则返回 0
if (res_set.count(item))
{
    // 对象存在
}
```

unordered_map
```c++
#include<unordered_map>
using std::unordered_map;

unordered_map<char, int> umap;

// umap[*iter] 如果 *iter 不存在, 会先存一个 *iter和对应默认值
umap[*iter] = umap[*iter] + 1;

// 是否找到, 不会添加新 key
umap.find(*iter) != umap.end();

// 遍历
for (auto iter = umap.begin(); iter != umap.end(); ++iter)
{
    cout << iter->first << ": " << iter->second << " ";
}
```