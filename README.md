# C++-11库 多线程编程
std::async
异步方式

条件变量 condition_variable
信令线程
1.互斥锁 mutex.lock() 或 std::lock_guard/ std::unique_lock(类名)
如：std::unique_lock<std::mutex> unique_lock(mutex)
2.释放锁 mutex.unlock() 或 std::lock_guard/ std::unique_lock

3. 条件变量cv 针对一个线程 cv.notify_one(); 全部 cv.notify_all();

等待线程
1. cv.wait(),cv.wait_for(),cv.wait_until()
