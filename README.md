# sqrt-x-

实现一个数的开方。

采用分治算法。

问题1：mid=left+(right-left)/2,而不是(left+right)/2?
问题2：判据形式为mid > x/ mid，而不是mid*mid>x

key idea:
若mid > x/ mid，令right=mid-1   //mid太大，最大为mid-1，则令right为mid-1
否则，若mid + 1 > x/ (mid + 1)，则返回mid,否则left=mid+1   
