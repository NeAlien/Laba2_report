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
echo "# timp-lab-02" >> README.md
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
