## Git

## init
- `.git' 폴더 생성하는 명렁어 (사진첩 생성)

```
git init
```
## status
- 현재 폴더의 git 작업상태
```
git status
```

## add
- staging area에 올리기 (무대에 올리기)
```
git add <file name>
git add . (모든 파일/폴더 올리기)
```


## commit
- `.git` repository에 저장 (사진찍기)
```
git commit -m "message"
```

## log
- git 히스토리 출력
``` 
git log (이 결과가 너무 길때는 q 를 눌러 나온다)
git log --oneline (필요한 핵심만 출력)
```

## remote
- 원격 저장소 주소를 별명 (origin)으로 추가
```
git remote add origin https://github.com/Joon1582/TIL.git
```
## push
- 원격 저장소에 업로드
```
git push origin main
```

