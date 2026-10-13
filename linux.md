# Linux

## 명령어 구조

- 셋 사이는 항상 **띄어쓰기**로 구분합니다
 - `brewinstall --cask iterm2`: 띄어쓰기 없이 쓰면 없는 명령어라고 나옴  
```
명령어 옵션 대상
ls   -l  notes
brew install --cask iterm2
```

## 경로

``은 코드로써 의미가 있는 것

- `~` : 내 홈 폴더를 의미한다  

- `.` : 지금 있는 폴더

- `..` : 한 칸 위 폴더 (상위 폴더)

- `/` 로 시작: 절대 경로 ex) 성동 캠퍼스 주소

- 나머지 : 상대 경로 ex) 장한평역에서 아래로 5분 걸어서 오면 돼

## 명령어

- pwd (print working directory) : 내가 작업중인 공간을 알려달라는 뜻. 내가 어느 파일에서 작업하고 있는지 알려줌. 

```
pwd
```

- ls (list) : 내가 어떤 파일이 있는지 확인하는 것. ls 는 밑에 하단 처럼 여러가지랑 붙혀서 쓸 수 있다
```
ls
ls TIL (TIL안에 파일 list 해줘)
ls -l (특정 폴더의 목록) (파일을 조금 더 자세히 보여주는 느낌)
ls -a (숨김 파일까지 보여준다) 숨김 파일: .으로 시작하는 파일/폴더
ls -la (숨김파일도 보여주면서 자세하게도 보여달라)
```

- cd (change directory) 디렉토리를 이동한다 (이동)
 - 파일이나 폴더는 tab으로 자동완성 사용 권장
```
cd .. (내가 현재 있는 폴더를 기준으로 한 단계 위로 올라가줘) 
cd ~ (홈으로 이동)
cd SD4/TIL (특정 폴더로 바로 이동)
```

- mrdir (make directory) 목적어가 없으면 의미가 없는 명령어
```
mkdir temp (temp라는 폴더 생성하는 명령어)
mkdir -p temp/hi (중간의 부모 폴더까지 만든는 명령어)
```
- touch (파일 생성)
```
touch
```

- echo (출력문, 프린트문) 메아리 준다
```
echo '안녕하세요'
```

- `>`(새로쓰기), `>>`(덧붙이기) 꺽쇠라고 하는 부등호를 쓰면 원하는 파일에 원하는 결과를 입력하도록 한다
```
echo 'hello' > test.txt (새로 쓴다. 만약 있으면 덮어쓴다)
echo 'world' >> test.txt (끝에 덧붙이기)
ls > test.txt (ls의 출력값을 text.txt에 쓰기)
```

- 파일 내용 보기
 - `cat` (전부출력)
 - `head -3`(앞부분 출력) (옵션을 입력하는 경우 그 줄만큼 보여준다)
 - `tail -2`(뒷부분 출력)
 - `less` (새로운 레이어에 출력)


- cp (copy), mv (move), rm (remove)
 - `rm -r` 폴더 삭제
```
cp test.txt temp (복사)
mv test.text temp2 (이동)
mv test.txt result.txt (이렇게 하면 이름 바꾸기가 된다. 같은 폴더에서 이동하는 경우에만)
rm result.txt (삭제) (result.txt라는 파일 삭제해줘라는 뜻) (파일만 삭제가능)
rm -r temp (-r 옵션은 폴더 삭제)
```

- `grep`, `\`
```
grep touch linux.md (linux.md 파일에서 touch가 들어간 줄 출력)
ls -l | grep linux (ls -l 출력결과 중에서 linux가 들어간 줄만 보기)
```

- which
 - 이 명령어가 어디있는지 출력 
```
which node (node명령어 위치)
```

- `--help` : 거의 대부분의 명령어 설명 출력



