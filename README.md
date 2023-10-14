# 四/八叉树

这个项目实现了一个简单的四叉树和八叉树，用于在三维空间中快速查找附近的物体。

这里只测试了简单的四叉树可视化，八叉树的可视化比较麻烦, 暂时没有测试.


1. 自定义DataType
   using Quad = QuadTree<Point, double>;
2. 通过lambda表达式, 自定义可视化func, 我在测试程序中提供了两种可视化方法
   void visual(std::function<void(Node* node)> func = nullptr) { traverse(root_, func);}