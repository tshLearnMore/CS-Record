* **剑指Offer**
   * 面试题1：[赋值运算符函数](#赋值运算符函数)
   * 面试题2：[实现Singleton模式](#实现Singleton模式)
   * 面试题3：[数组中重复的数字](#数组中重复的数字)
   * 面试题4：[二维数组的查找](#二维数组的查找)
   * 面试题5：[替换空格](#替换空格)
   * 面试题6：[从头到尾打印链表](#从头到尾打印链表)
   * 面试题7：[重建二叉树](#重建二叉树)
   * 面试题8：[二叉树的下一个节点](#二叉树的下一个节点)
   * 面试题9：[用两个栈实现队列](#用两个栈实现队列)
   * 面试题10：[裴波那契数列](#裴波那契数列)
   * 面试题11：[旋转数组的最小数字](#旋转数组的最小数字)
   * 面试题12：[矩阵中的路径](#矩阵中的路径)
   * 面试题13：[机器人的运动范围](#机器人的运动范围)
   * 面试题14：[剪绳子](#剪绳子)
   * 面试题15：[二进制中1的个数](#二进制中1的个数)
   * 面试题16：[数值的整数次方](#数值的整数次方)
   * 面试题17：[打印从1到最大的n位数](#打印从1到最大的n位数)
   * 面试题18：[删除链表的节点](#删除链表的节点)
   * 面试题19：[正则表达式匹配](#正则表达式匹配)
   * 面试题20：[表示数值的字符串](#表示数值的字符串)
   * 面试题21：[调整数组顺序使奇数位于偶数前面](#调整数组顺序使奇数位于偶数前面)
   * 面试题22：[链表中倒数第k个节点](#链表中倒数第k个节点)
   * 面试题23：[链表中环的入口节点](#链表中环的入口节点)
   * 面试题24：[反转链表](#反转链表)
   * 面试题25：[合并两个排序的链表](#合并两个排序的链表)
   * 面试题26：[树的子结构](#树的子结构)
   * 面试题27：[二叉树的镜像](#二叉树的镜像)
   * 面试题28：[对称的二叉树](#对称的二叉树)
   * 面试题29：[顺时针打印矩阵](#顺时针打印矩阵)
   * 面试题30：[包含min函数的栈](#包含min函数的栈)
   * 面试题31：[栈的压入弹出序列](#栈的压入弹出序列)
   * 面试题32：[从上到下打印二叉树](#从上到下打印二叉树)
   * 面试题33：[二叉搜索树的后序遍历序列](#二叉搜索树的后序遍历序列)
   * 面试题34：[二叉树中和为某一值的路径](#二叉树中和为某一值的路径)
   * 面试题35：[复杂链表的复制](#复杂链表的复制)
   * 面试题36：[二叉搜索树与双向链表](#二叉搜索树与双向链表)
   * 面试题37：[序列化二叉树](#序列化二叉树)
   * 面试题38：[字符串的排列](#字符串的排列)
   * 面试题39：[数组中出现次数超过一半的数字](#数组中出现次数超过一半的数字)
   * 面试题40：[最小的k个数](#最小的k个数)
   * 面试题41：[数据流中的中位数](#数据流中的中位数)
   * 面试题42：[连续子数组的最大和](#连续子数组的最大和)
   * 面试题43：[1~n整数中1出现的次数](#1n整数中1出现的次数)
   * 面试题44：[数字序列中某一位的数字](#数字序列中某一位的数字)
   * 面试题45：[把数组排成最小的数](#把数组排成最小的数)
   * 面试题46：[把数字翻译成字符串](#把数字翻译成字符串)
   * 面试题47：[礼物的最大价值](#礼物的最大价值)
   * 面试题48：[最长不含重复字符的子字符串](#最长不含重复字符的子字符串)
   * 面试题49：[丑数](#丑数)
   * 面试题50：[第一个只出现一次的字符](#第一个只出现一次的字符)
   * 面试题51：[数组中的逆序对](#数组中的逆序对)
   * 面试题52：[两个链表的第一个公共节点](#两个链表的第一个公共节点)
   * 面试题53：[在排序数组中查找数字](#在排序数组中查找数字)
   * 面试题54：[二叉搜索树的第k大节点](#二叉搜索树的第k大节点)
   * 面试题55：[二叉树的深度](#二叉树的深度)
   * 面试题56：[数组中数字出现的次数](#数组中数字出现的次数)
   * 面试题57：[和为s的数字](#和为s的数字)
   * 面试题58：[翻转字符串](#翻转字符串)
   * 面试题59：[队列的最大值](#队列的最大值)
   * 面试题60：[n个骰子的点数](#n个骰子的点数)
   * 面试题61：[扑克牌中的顺子](#扑克牌中的顺子)
   * 面试题62：[圆圈中最后剩下的数字](#圆圈中最后剩下的数字)
   * 面试题63：[股票的最大利润](#股票的最大利润)
   * 面试题64：[求1~n的和](#求1n的和)
   * 面试题65：[不用加减乘除做加法](#不用加减乘除做加法)
   * 面试题66：[构建乘积数组](#构建乘积数组)
   
# 剑指Offer题解
## 赋值运算符函数

```
//先创建一个临时实例，然后交换临时实例和原来的实例
CMyString& CMyString::operator =(const CMyString& str)
{
	if (this != &str)
	{
		CMyString temp(str);
		
		char* pTemp = temp.pData_;
		temp.pData_ = pData_;
		pData_ = pTemp;
	}
	return *this;
}

```
## 实现Singleton模式

```
//第一种懒汉式单例
class SingleClass
{
public:
	static SingleClass* GetInstance()
	{
		if (!instance)
			instance = new SingleClass();
		return instance;
	}

private:
	SingleClass(){};
	static SingleClass *instance;
};

SingleClass * SingleClass::instance = NULL;

---------------------------------------------

//第二种局部静态变量单例
class SingleClass
{
private:
	SingleClass() { }
	SingleClass(const SingleClass &);
	SingleClass & operator = (const SingleClass &);
public:
	static SingleClass* GetInstance()
	{
		static SingleClass instance;
		return &instance;
		//返回指针。返回引用的话，因为外部可能Singleton singleton = Singleton :: GetInstance();产生一次拷贝
	}
};


```

## 数组中重复的数字

```
//题目描述：在一个长度为n的数组里的所有数字都在0到n-1的范围内。
数组中某些数字是重复的，但不知道有几个数字是重复的。也不知道每个数字重复几次。
请找出数组中任意一个重复的数字。 例如，如果输入长度为7的数组{2,3,1,0,2,5,3}，
那么对应的输出是第一个重复的数字2。
//思路：重排数组，扫描数字num[i]是否等于i，若果是则扫描下一个；如果不是则拿它和第num[i]个数字比较，要是相等则找到一个重复数字，要是不相等则交换位置，直到第i位置上找到正确的数字；重复这个比较
bool duplicate(int numbers[], int length, int* duplication) {
	if(length < 0 || numbers == NULL)
		return false;
	for(int i = 0; i < length; i++)
	{
		while(numbers[i] != i)
		{
			if (numbers[numbers[i]] == numbers[i])
			{
				*duplication = numbers[i];
				return true;
			}
			swap(numbers[i],numbers[numbers[i]]);
		}
	}
	return false;
}

```

## 二维数组的查找

```
//题目：在一个二维数组中（每个一维数组的长度相同），每一行都按照从左到右递增的顺序排序，
每一列都按照从上到下递增的顺序排序。请完成一个函数，输入这样的一个二维数组和一个整数，
判断数组中是否含有该整数。
//思路：从右上角开始判断
1.若arr[row][col]==target,则找到
2.若arr[row][col] >target,则col--
3.若arr[row][col] <target,则row++

bool Find(int target, vector<vector<int> > arr) {
	int row = arr.size() - 1;
	if (row < 0)
	{
		return false;
	}
	int col = arr[0].size() - 1;

	int rowBound = 0;
	int colBound = col;

	while (rowBound <= row && colBound >=0)
	{
		if (arr[rowBound][colBound] == target)
		{
			return true;
		}
		if (arr[rowBound][colBound] > target)
		{
			colBound--;
		}
		if (arr[rowBound][colBound] < target)
		{
			rowBound++;
		}
	}
	return false;
}

```

## 替换空格
```
//题目：请实现一个函数，将一个字符串中的每个空格替换成“%20”。例如，当字符串为We Are Happy.
则经过替换之后的字符串为We%20Are%20Happy
//思路：
1.先计算空格个数spaceNum，
2.然后计算出替换空格后总长度length=str.size()+2*spaceNum
3.从后往前替换空格

void replaceSpace(char *str,int length) {
	if(str==NULL || length<=0)
		return;
	int oldLength = 0;
	int newLength = 0;
	int spaceNum = 0;
	for(int i = 0;str[i]!='\0';i++)
	{
		oldLength++;
		if(str[i] == ' ')
			spaceNum++;
	}
	newLength=oldLength+spaceNum*2;
	if(length < newLength+1)
		return;//原始位置容量不够
	for(int len = oldLength;len >= 0;len--)
	{
		if(str[len] == ' ')
		{
			str[newLength--]='0';
			str[newLength--]='2';
			str[newLength--]='%';
		}
		else
			str[newLength--]=str[len];
	}
}
```
## 从头到尾打印链表
```
//题目：输入一个链表，按链表值从尾到头的顺序返回一个ArrayList。
//思路：1.一种是用栈保存 2.另一种是递归
    vector<int> printListFromTailToHead(ListNode* head) {
        vector<int> re;
        insertNode(re,head);
        return re;
    }
    void insertNode(vector<int>& vec,ListNode* head)
    {
        if(head!=NULL)
        {
            insertNode(vec,head->next);
            vec.push_back(head->val);
        }
    }
```
## 重建二叉树
```
//题目：输入某二叉树的前序遍历和中序遍历的结果，请重建出该二叉树。假设输入的前序遍历和
中序遍历的结果中都不含重复的数字。例如输入前序遍历序列{1,2,4,7,3,5,6,8}和中序遍历序列
{4,7,2,1,5,3,8,6}，则重建二叉树并返回。
//思路：
1.以前序遍历的第一个值，即根节点，将数组分成两半
2.然后递归分别处理这两边。
注意截止条件：数组长度为0则停止递归

TreeNode* buildTree(vector<int>& pre,vector<int>& vin,int preLeft,int preRight,int vinLeft,int vinRight)
{
	if (preLeft > preRight || vinLeft > vinRight)
		return NULL;
	TreeNode* root = new TreeNode(pre[preLeft]);
	int pos=vinLeft;
	while (pos<=vinRight&&vin[pos]!=pre[preLeft])
		pos++;
	int diff = pos - vinLeft;
	if(pos - vinLeft)
		root->left=buildTree(pre,vin,preLeft+1,preLeft+diff,vinLeft,vinLeft+diff-1);
	if(vinRight - pos)
		root->right=buildTree(pre,vin,preLeft+diff+1,preRight,vinLeft+diff+1,vinRight);
	return root;
}

TreeNode* reConstructBinaryTree(vector<int> pre,vector<int> vin) {
	if (pre.size()!=vin.size())
		return NULL;
	return buildTree(pre,vin,0,pre.size()-1,0,vin.size()-1);
}

```

## 二叉树的下一个节点
```
//题目：给定一个二叉树和其中的一个结点，请找出中序遍历顺序的下一个结点并且返回。
注意，树中的结点不仅包含左右子结点，同时包含指向父结点的指针。
//思路：
1.节点有右子树，它的下一个节点就是它右子树的最左节点
2.节点没有右子树
  2.1是它父节点的左子树，下一个节点就是父节点
  2.2是它父节点的右子树，沿着父节点向上遍历，直到找到一个是它父节点左子树节点的节点。
     如果这样的节点存在，则这个节点的父节点就是要找的节点

TreeLinkNode* GetNext(TreeLinkNode* pNode)
{
	if(pNode==NULL)
		return NULL;
	TreeLinkNode* re=NULL;
	//节点有右子树
	if (pNode->right!=NULL)
	{
		re=pNode->right;
		while(re->left!=NULL)
			re=re->left;
		return re;
	}
	if (pNode->next!=NULL)
	{
		//节点是父节点的左子树
		if (pNode==pNode->next->left)
			return pNode->next;
		//节点是父节点的右子树
		TreeLinkNode* parent=pNode->next;
		while (parent->next!=NULL&&parent!=parent->next->left)
			parent=parent->next;
		if(parent->next!=NULL&&parent==parent->next->left)
			re = parent->next;
		return re;
	}
	return re;
}

```
## 用两个栈实现队列
```
//题目：用两个栈来实现一个队列，完成队列的Push和Pop操作。 队列中的元素为int类型。
//思路：
1.只有stack1保存数据，stack2一直为空
2.push只push到stack1中
2.pop操作，先压栈到stack2中直到stack1中还剩一个为止，这个数就是要实际pop的。再将
stack2中数据push到stack1中

class Solution
{
public:
	void push(int node) {
		stack1.push(node);
	}

	int pop() {
		int value=-1;
		while (!stack1.empty())
		{
			if (stack1.size()==1)
				value=stack1.top();
			else
				stack2.push(stack1.top());
			stack1.pop();
		}
		while (!stack2.empty())
		{
			stack1.push(stack2.top());
			stack2.pop();
		}
		return value;
	}

private:
	stack<int> stack1;
	stack<int> stack2;
};

```
## 裴波那契数列
```
//思路：f(n) = f(n-1) + f(n-2)

int Fibonacci(int n) {
	if (n < 0)
		return -1;
	if (n == 0)
		return 0;
	int fn_one=1;
	int fn_two=0;
	int fn=1;
	for(int i = 2;i <= n;i++)
	{
		fn = fn_one + fn_two;
		fn_two = fn_one;
		fn_one = fn;
	}
	return fn;
}
```
## 旋转数组的最小数字
```
//题目：把一个数组最开始的若干个元素搬到数组的末尾，我们称之为数组的旋转。 
输入一个非减排序的数组的一个旋转，输出旋转数组的最小元素。 
例如数组{3,4,5,1,2}为{1,2,3,4,5}的一个旋转，该数组的最小值为1。 
NOTE：给出的所有元素都大于0，若数组大小为0，请返回0。
//思路：
1.如果数组的第一个数字小于最后一个，说明数组没发生旋转，直接返回rotate[0]
2.如果rotate[start]==rotate[mid]==rotate[end],说明数组中数字有重复，最小数字落在start和end之间，让start++，进入下一次循环。这里的最坏情况是O(n)
3.如果rotate[start]<=rotate[mid],则最小数字在后半部分
4.如果rotate[mid]<=rotate[end],则最小数字在前半部分

int minNumberInRotateArray(vector<int> rotateArray) {
	if (rotateArray.size()==0)
		return -1;
	int start=0;
	int end=rotateArray.size()-1;
	int ret = rotateArray[0];
	while (ret>=rotateArray[end])
	{
		if (end-start==1)
			return rotateArray[end];
		int mid = (end+start)/2;
		if (rotateArray[start]==rotateArray[mid]&&rotateArray[mid]==rotateArray[end])
			start++;//这里可以直接用find查找start到end之间的最小值
		else if (rotateArray[start]<=rotateArray[mid])
			start=mid;
		else if (rotateArray[mid]<= rotateArray[end])
			end=mid;
	}
	return ret;
}

```
## 矩阵中的路径
```
//题目：请设计一个函数，用来判断在一个矩阵中是否存在一条包含某字符串所有字符的路径。
路径可以从矩阵中的任意一个格子开始，每一步可以在矩阵中向左，向右，向上，向下移动一个格子。
如果一条路径经过了矩阵中的某一个格子，则之后不能再次进入这个格子。 
例如 a b c e s f c s a d e e 这样的3 X 4 矩阵中包含一条字符串"bcced"的路径，
但是矩阵中不包含"abcb"路径，因为字符串的第一个字符b占据了矩阵中的第一行第二个格子之后，路径不能再次进入该格子。
//思路：
1.外部循环尝试每个位置为起点
2.实际查找是尝试上下左右四个方向，并将访问过的节点设为true，退出时设为false

bool findPath(char* matrix, bool* state,int x, int y,int rows, int cols, char* str)
{
    if (*str == '\0')
		return true;
	if (x<0||x>=rows||y<0||y>=cols)
		return false;
	if (*str != *(matrix+(x*cols+y)) || *(state+(x*cols+y))==true)
		return false;
	*(state+(x*cols+y))=true;
	bool ret = findPath(matrix,state,x-1,y,rows,cols,str+1);
	if (!ret)
		ret = findPath(matrix,state,x+1,y,rows,cols,str+1);
	if (!ret)
		ret = findPath(matrix,state,x,y-1,rows,cols,str+1);
	if (!ret)
		ret = findPath(matrix,state,x,y+1,rows,cols,str+1);
	*(state+(x*cols+y))=false;
	return ret;
}

bool hasPath(char* matrix, int rows, int cols, char* str)
{
	if (matrix==NULL||str==NULL)
		return false;
	bool* state = new bool[rows*cols];
	memset(state,0,rows*cols);
	for (int i=0;i<rows;i++)
		for (int j=0;j<cols;j++)
			if (findPath(matrix,state,i,j,rows,cols,str))
            {
                delete[] state;
                return true;
            }
    delete[] state;
	return false;
}
```
## 机器人的运动范围
```
//题目：地上有一个m行和n列的方格。一个机器人从坐标0,0的格子开始移动，每一次
只能向左，右，上，下四个方向移动一格，但是不能进入行坐标和列坐标的数位之和大于k的格子。 
例如，当k为18时，机器人能够进入方格（35,37），因为3+5+3+7 = 18。但是，
它不能进入方格（35,38），因为3+5+3+8 = 19。请问该机器人能够达到多少个格子？
//思路：和上一题思路类似，只是有一个进入条件的判断
bool judge(int rows,int cols,int thr)
{
	int num = 0;
	while(rows)
	{
		num+=rows%10;
		rows=rows/10;
	}
	while(cols)
	{
		num+=cols%10;
		cols=cols/10;
	}
	if (thr<num)
		return false;
	else
		return true;
}

void findPath(vector<vector<bool>>& arr,int rows,int cols,int x,int y,int threshold,int* num)
{
	if (x<0||x>=rows||y<0||y>=cols)
		return ;
	if (!judge(x,y,threshold) || arr[x][y]==true)
		return ;
	arr[x][y]=true;
	*num = *num + 1;
	findPath(arr,rows,cols,x-1,y,threshold,num);
	findPath(arr,rows,cols,x+1,y,threshold,num);
	findPath(arr,rows,cols,x,y-1,threshold,num);
	findPath(arr,rows,cols,x,y+1,threshold,num);
}

int movingCount(int threshold, int rows, int cols)
{
	vector<vector<bool>> arr;
	for (int i=0;i<rows;i++)
	{
		vector<bool> temp;
		for (int j=0;j<cols;j++)
			temp.push_back(false);
		arr.push_back(temp);
	}
	int num=0;
	findPath(arr,rows,cols,0,0,threshold,&num);
	return num;
}


```
## 剪绳子
## 二进制中1的个数
## 数值的整数次方
## 打印从1到最大的n位数
## 删除链表的节点
## 正则表达式匹配
## 表示数值的字符串
## 调整数组顺序使奇数位于偶数前面
## 链表中倒数第k个节点
## 链表中环的入口节点
## 反转链表
## 合并两个排序的链表
## 树的子结构
## 二叉树的镜像
## 对称的二叉树
## 顺时针打印矩阵
## 包含min函数的栈
## 栈的压入弹出序列
## 从上到下打印二叉树
## 二叉搜索树的后序遍历序列
## 二叉树中和为某一值的路径
## 复杂链表的复制
## 二叉搜索树与双向链表
## 序列化二叉树
## 字符串的排列
## 数组中出现次数超过一半的数字
## 最小的k个数
## 数据流中的中位数
## 连续子数组的最大和
## 1~n整数中1出现的次数
## 数字序列中某一位的数字
## 把数组排成最小的数
## 把数字翻译成字符串
## 礼物的最大价值
## 最长不含重复字符的子字符串
## 丑数
## 第一个只出现一次的字符
## 数组中的逆序对
## 两个链表的第一个公共节点
## 在排序数组中查找数字
## 二叉搜索树的第k大节点
## 二叉树的深度
## 数组中数字出现的次数
## 和为s的数字
## 翻转字符串
## 队列的最大值
## n个骰子的点数
## 扑克牌中的顺子
## 圆圈中最后剩下的数字
## 股票的最大利润
## 求1~n的和
## 不用加减乘除做加法
## 构建乘积数组
