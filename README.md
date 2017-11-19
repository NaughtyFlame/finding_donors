# 练习项目：为CharityML寻找捐助者
### 安装
这个项目使用Python3.6并且需要安装下面这些python库：
* Python 3.6
* Numpy
* Pandas
* scikit-learn
* matplotlib
同样需要安装好相应的软件才能运行 [iPython Notebook](http://ipython.org/notebook.html)

### 说明
这是一个[Udacity](cn.udacity.com)机器学习的[课程项目](https://github.com/nd009/finding_donors)，在完成之后进行了整理、改进和优化。

主要的代码包含在`finding_donors.ipynb`这个notebook文件中。还会用到[visuals.py]()这个可视化辅助文件，和名为`census.csv`的数据文件。

### 数据
修改的人口普查数据集含有将近32,000个数据点，每一个数据点含有13个特征。这个数据集是Ron Kohavi的论文 *"Scaling Up the Accuracy of Naive-Bayes Classifiers: a Decision-Tree Hybrid"*,中数据集的一个修改版本。你能够在[这里](https://www.aaai.org/Papers/KDD/1996/KDD96-033.pdf)找到论文，在[UCI的网站](https://archive.ics.uci.edu/ml/datasets/Census+Income)找到原始数据集。

#### 特征

* age: 一个整数，表示被调查者的年龄。
* workclass: 一个类别变量表示被调查者的通常劳动类型，允许的值有 {Private, Self-emp-not-inc, Self-emp-inc, Federal-gov, Local-gov, State-gov, Without-pay, Never-worked}
* education_level: 一个类别变量表示教育程度，允许的值有 {Bachelors, Some-college, 11th, HS-grad, Prof-school, Assoc-acdm, Assoc-voc, 9th, 7th-8th, 12th, Masters, 1st-4th, 10th, Doctorate, 5th-6th, Preschool}
* education-num: 一个整数表示在学校学习了多少年
* marital-status: 一个类别变量，允许的值有 {Married-civ-spouse, Divorced, Never-married, Separated, Widowed, Married-spouse-absent, Married-AF-spouse}
* occupation: 一个类别变量表示一般的职业领域，允许的值有 {Tech-support, Craft-repair, Other-service, Sales, Exec-managerial, Prof-specialty, Handlers-cleaners, Machine-op-inspct, Adm-clerical, Farming-fishing, Transport-moving, Priv-house-serv, Protective-serv, Armed-Forces}
* relationship: 一个类别变量表示家庭情况，允许的值有 {Wife, Own-child, Husband, Not-in-family, Other-relative, Unmarried}
* race: 一个类别变量表示人种，允许的值有 {White, Asian-Pac-Islander, Amer-Indian-Eskimo, Other, Black}
* sex: 一个类别变量表示性别，允许的值有 {Female, Male}
* capital-gain: 连续值。
* capital-loss: 连续值。
* hours-per-week: 连续值。
* native-country: 一个类别变量表示原始的国家，允许的值有 {United-States, Cambodia, England, Puerto-Rico, Canada, Germany, Outlying-US(Guam-USVI-etc), India, Japan, Greece, South, China, Cuba, Iran, Honduras, Philippines, Italy, Poland, Jamaica, Vietnam, Mexico, Portugal, Ireland, France, Dominican-Republic, Laos, Ecuador, Taiwan, Haiti, Columbia, Hungary, Guatemala, Nicaragua, Scotland, Thailand, Yugoslavia, El-Salvador, Trinadad&Tobago, Peru, Hong, Holand-Netherlands}
#### 目标变量

*income: 一个类别变量，表示收入属于那个类别，允许的值有 {<=50K, >50K}