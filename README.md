# GraceBlog
numpy:www.numpy.org

1.安全转换数据类型 : astype

        a = np.array([[1,2,3,4], [4,5,6,7], [4,5,8,9]], dtype=np.float)
        print(a.shape)
        print(a)
        b = a.astype(np.int)
        print(b)

        (3, 4)
        [[1. 2. 3. 4.]
         [4. 5. 6. 7.]
         [4. 5. 8. 9.]]
        [[1 2 3 4]
         [4 5 6 7]
         [4 5 8 9]]
2. numpy的类型：np.float, np.complex, np.int

3. e1 = np.arange(1,10,0.5)
    print(e1)
    
    [1.  1.5 2.  2.5 3.  3.5 4.  4.5 5.  5.5 6.  6.5 7.  7.5 8.  8.5 9.  9.5]

4.linspace: 函数通过指定起始值、终止值和元素个数来创建数组，缺省包括终止值
  b = np.linspace(1,10,10)
  print('b=',b)
  b= [ 1.  2.  3.  4.  5.  6.  7.  8.  9. 10.]
  endpoint=False: 不包括终止值
 

         5. # 1： 10^1, 2:10^2;  9: 9个数
                # 如果base=2 则 表示2^1, 2^2
                d = np.logspace(1,2,9, endpoint=True, base=2)
                print(d)
                        [2.         2.18101547 2.37841423 2.59367911 2.82842712 3.08442165
                        3.36358566 3.66801617 4.        ]

        6. 切片数据是原数组的一个视图，与原数组共享内容空间，可以直接修改元素值
                a = np.arange(10)
                print(a)
                a[1:4] = 10,20,30
                print(a)
                [0 1 2 3 4 5 6 7 8 9]
                [ 0 10 20 30  4  5  6  7  8  9]
