# Laba2_report-TiMP

## Part I
Задание №1
```
https://github.com/NeAlien/Laba2
```
Задание №2
```
mkdir Laba2
cd Laba2
echo "# Laba2" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/NeAlien/Laba2.git
git push -u origin master
```
Задание №3
```
cat > "Hello_world.cpp" << EOF
#include <iostream>

using namespace std;
int main(int argc, char** argv){
 cout << "Hello world" << endl;
}
EOF
```
Задание №4
```
git add "Hello_world.cpp"
```
Задание №5
```
git commit -m "Added new cpp file"
```
Задание №6
```
alias edit=nano
edit "Hello world.cpp"
 #include <iostream>
 #include <string>
 
 using namespace std;
 int main(int argc, char** argv){
  string name;
  cin >> name;
  cout << "Hello world from " << name << endl;
 }
```
Задание №7
```
git commit -a -m "Changed cpp file"
```
Задание №8
```
git push -u origin master
```
Задание №9
```
История коммитов доступна в удалёном репозитории
```

## Part II
Задание №1
```
git checkout -b patch1
```
Задание №2
```
edit "Hello_world.cpp"
#include <iostream>
#include <string>
 
int main(int argc, char** argv){
 string name;
 std::cin >> name;
 std::cout << "Hello world from " << name << std::endl;
}
```
Задание №3
```
git commit -a -m "Fixed cpp file"
git push -u origin patch1
```
Задание №4
```
Ветка patch1 доступна в удалённом репозитории
```
Задание №5
```
Создадим pull-request patch1 -> master
```
Задание №6
```
edit "Hello_world.cpp"
#include <iostream>
#include <string>
 
int main(int argc, char** argv){
 string name; \\ User name
 std::cin >> name; \\ Input user name
 std::cout << "Hello world from " << name << std::endl;
} 
```
Задание №7
```
git commit -a -m "Added comments"
git push -u origin patch1
```
Задание №8
```
Новые изменения есть в созданном на шаге 5 pull-request
```
Задание №9
```
 В удалённом репозитории выполняем слияние PR patch1 -> master и удаляем ветку patch1 в удаленном репозитории.
```
Задание №10
```
git pull origin
```
Задание №11
```
git log
```
Задание №12
```
git branch -D patch1
```
## Part III
Задание №1
```
git checkout -b patch2
```
Задание №2
```
clang-format -i -style=Mozilla "Hello_world.cpp"
```
Задание №3
```
git commit -a -m "Changed code style in cpp file"
git push -u origin patch2
```
Задание №4
```
В ветке master в удаленном репозитории изменяем комментарии

#include <iostream>
#include <string>
 
int main(int argc, char** argv){
 string name; \\ User n.
 std::cin >> name; \\ Ввод данных
 std::cout << "Hello world from " << name << std::endl;
}  
```
Задание №5
```
Убеждаемся, что в pull-request появились конфликтны.
```
Задание №6
```
git pull origin master
git rebase master
edit "Hello world.cpp"
git commit -a -m "Update Hello world.cpp"
git rebase --continue
```
Задание №7
```
git push -f origin patch2
```
Задание №8
```
Убеждаемся, что в pull-request пропали конфликтны.
```
Задание №9
```
Выполняем merge pull-request patch2 -> master
```
