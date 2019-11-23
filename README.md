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
