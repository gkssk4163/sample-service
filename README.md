
## Create Helm chart 
1. git repository checkout 및 stable 디렉토리 생성
```
git checkout  https://github.com/yoonjk/sample-service.git
cd sample-service & mkdir stable
```

2. demo helm chart 생성 및 package
```
helm create sample

# helm package demo
3. helm 파일을 stable 디렉토리에 복사
```
mv sample-0.1.0.tgz stable
```

4. Index 파일 생성
```
helm repo index [INDEX_FILE_PATH] --url [CHART_REPO_URL]
helm repo index stable --url https://yoonjk.github.io/sample-service/stable
```

5. git에 commit and push
```
git add --all & git commit -m 'First Commit' & git push origin master
```

