---
layout: post
title: "favicon"
comments: true
# other options
---


1. https://icons8.kr/icons/set/favicon-ico 에서 원하는 favicon 이미지를 16x16으로 다운받는다

2. 루트 디렉토리에 asset 폴더를 새롭게 만들고 다운받는 이미지를 넣는다


3. /_config.yml 에 코드 asset_url: /assets 추가한다

2. /_include/head.html 12라인 favicon 설정하는 코드를 추가한다 
<link href="{{ site.asset_url }}/favicon.png" rel="shortcut icon" type="image/vnd.microsoft.icon"/>
