# Assignment Week 2:

You needn't finish reading all of them in just one week!
It's just good for you to know what's happening in this area and to figure out how people try to improve SIFT.

You needn't to remember all of them. 
But please DO REMEMBER procedures of SIFT and HoG. For those who're interested in SLAM, Orb is your inevitable destiny.

# [Reading]:

1. [optional] Bilateral Filter: https://blog.csdn.net/piaoxuezhong/article/details/78302920

2. Feature Descriptors:

   [Compulsory]
   
   Hog: https://lear.inrialpes.fr/people/triggs/pubs/Dalal-cvpr05.pdf
   
   SURF: https://www.vision.ee.ethz.ch/~surf/eccv06.pdf
   
# [Coding]:			
1. 
    Finish 2D convolution/filtering by your self. 
    What you are supposed to do can be described as "median blur", which means by using a sliding window 
    on an image, your task is not going to do a normal convolution, but to find the median value within 
    that crop.

    You can assume your input has only one channel. (a.k.a a normal 2D list/vector)
    And you do need to consider the padding method and size. There are 2 padding ways: REPLICA & ZERO. When 
    "REPLICA" is given to you, the padded pixels are same with the border pixels. E.g is [1 2 3] is your
    image, the padded version will be [(...1 1) 1 2 3 (3 3...)] where how many 1 & 3 in the parenthesis 
    depends on your padding size. When "ZERO", the padded version will be [(...0 0) 1 2 3 (0 0...)]

    Assume your input's size of the image is W x H, kernel size's m x n. You may first complete a version 
    with O(W·H·m·n log(m·n)) to O(W·H·m·n·m·n)).
    Follow up 1: Can it be completed in a shorter time complexity?

    Python version:
    def medianBlur(img, kernel, padding_way):
        img & kernel is List of List; padding_way a string
        Please finish your code under this blank


高斯模糊的算法 -- https://blog.csdn.net/dcrmg/article/details/52304446

怎样更好地理解并记忆泰勒展开式？ -- https://www.zhihu.com/question/25627482
