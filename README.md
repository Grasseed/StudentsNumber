# 學生座號姓名
    輸入 0~5 (ex:1)
    輸出 錢一文
    (請參考表1)
| 座號  | 學生姓名  | 陣列元素 |
| :------------ |:---------------:| -----:|
| 1 | 錢一文 | name[0] |
| 2 | 孫二娘 | name[1] |
| 3 | 張三豐 | name[2] |
| 4 | 李四維 | name[3] |
| 5 | 李四維 | name[4] |
    表1
```cs
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace StudentsNumber
{
    class Program
    {
        static void Main(string[] args)
        {
            string[] name = new string[] {"錢一文","孫二娘","張三豐","李四維","王五金"};
            int i = int.Parse(Console.ReadLine());
            if(i>=1 && i<=5)
            {
                Console.WriteLine("學生姓名:{0}", name[i - 1]);
            }
            //陣列與元素的標示兩者差一
            else
            {
                Console.WriteLine("...這是空號...");
            }
            Console.Read();
        }
    }
}

```
