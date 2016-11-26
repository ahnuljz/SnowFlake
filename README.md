# SnowFlake
Twitter的雪花算法SnowFlake，使用Java语言实现。

SnowFlake算法用来生成64位的ID，刚好可以用long整型存储，能够用于分布式系统中生产唯一的ID， 并且生成的ID有大致的顺序。
在这次实现中，生成的64位ID可以分成5个部分：

  0 - 41位时间戳 - 5位数据中心标识 - 5位机器标识 - 12位序列号
  
5位数据中心标识跟5位机器标识这样的分配仅仅是当前实现中分配的，如果业务有其实的需要，可以按其它的分配比例分配，如10位机器标识，不需要数据中心标识。

生成的ID如下所示：
2099698216983
2099698216984
2099698216985
2099698216986
2099698216987
2099698216988
2099698216989
2099698216990
2099698216991
2099698216992
2099698216993
2099698216994
2099698216995
2099698216996
2099698216997
2099698216998
2099698216999
2099698217000
2099698217001
2099698217002
2099698217003
2099698217004
2099698217005
2099698217006
2099698217007
2099698217008
2099698217009
2099698217010
2099698217011
2099698217012
2099698217013
2099698217014
2099698217015
2099698217016
2099698217017
2099698217018
2099698217019
2099698217020
2099698217021
2099698217022
2099698217023
2099698217024
2099698217025
2099698217026
2099698217027
2099698217028
2099698217029
2099698217030
2099698217031
2099702411264
2099702411265
2099702411266
2099702411267
2099702411268
2099702411269
2099702411270
2099702411271
2099702411272
2099702411273
2099702411274
2099702411275
2099702411276
2099702411277

