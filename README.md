# tensorflow_notes

1.ExponentialMovingAverage : 首先Moving average 就是滑动取平均. 指数指的是当前值和前面值是一个指数的比例. 这里为了避免参数变动很大，提出了这个方法.可能在当前步对于Loss来看是最优的,但是整体来看就不一定了. 这个在训练过程中，每次都是用ExponentialMovingAverage后的值作为当前的值.刚开始想训练的快一些，可以将decay参数调的低一些,到后面再调高. 在测试的过程中,也是用这个值来做预测.
       
    参考:https://www.reddit.com/r/tensorflow/comments/5zsc5g/what_does_moving_average_do_when_training_a/  以及书籍

2. tensorflow 性能分析:  http://walsvid.github.io/2017/03/25/profiletensorflow/
