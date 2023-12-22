## client
npx create-react-app .   
npm install sass   
npm install react-bootstrap bootstrap   
npm install react-router-dom   
npm install axios   
npm install http-proxy-middleware   
npm install @emotion/css    
npm install @emotion/react  
npm install @emotion/styled   
npm install firebase   
npm install react-redux   
npm install @reduxjs/toolkit   
npm install react-avatar
npm install moment

## server
npm init -y;   
npm install express --save;   
npm install nodemon --save;   
npm install path --save;   
npm install mongoose --save;   
npm install multer --save;      
npm install aws-sdk@2.348.0 --save;      
npm install multer-s3@2.10.0 --save;      

## 문제 해결
- client 폴더에 화살표 생길 때 : .git 폴더를 지운다.   
`rm -rf .git`   
`git rm --cached . -rf`# simple300   


## 라이브러리
1. moment
moment 명령은 Node.js 프로젝트에서 JavaScript 라이브러리인 "moment.js"를 설치하는 명령입니다. "moment.js"는 날짜와 시간을 처리하는 JavaScript 라이브러리로, 날짜와 시간을 쉽게 다루고 포맷팅하는데 도움을 줍니다.

위 명령을 실행하면 현재 프로젝트 디렉토리에 "moment" 라이브러리가 설치됩니다. 이후에 프로젝트의 JavaScript 파일에서 "moment" 라이브러리를 사용할 수 있게 됩니다.

일반적으로 프로젝트에서 필요한 라이브러리를 설치하기 위해 npm install 명령을 사용합니다. 이 명령은 프로젝트의 종속성(dependencies)을 관리하고 필요한 라이브러리를 프로젝트에 추가하는 데 사용됩니다.

2. avatar
npm install react-avatar 명령은 React 애플리케이션에서 사용할 수 있는 프로필 이미지 및 아바타(avatar)를 만들기 위한 React 컴포넌트 라이브러리인 "react-avatar"를 설치하는 명령입니다.

"react-avatar" 라이브러리를 사용하면 개발자들은 사용자 프로필 이미지, 그룹 아바타, 댓글 작성자의 이미지 등과 같은 아바타 이미지를 생성하고 표시하는 데 도움을 받을 수 있습니다. 이 라이브러리를 사용하면 이미지 크기, 모양, 색상 등을 설정할 수 있는 많은 옵션이 제공됩니다.

예를 들어, 다음과 같이 "react-avatar"를 사용하여 프로필 이미지를 생성할 수 있습니다:#   R E A C T - B L O G 
 
 #   R E A C T - B L O G 
 
 #   R E A C T - B L O G 
 
## 클라이언트(Client)
npx create-react-app . : 현재 디렉토리에 React 앱을 생성합니다.
npm install react-bootstrap bootstrap : React에서 사용할 수 있는 Bootstrap 패키지를 설치합니다.
npm install react-router-dom : React 앱에서 라우팅을 관리하기 위한 패키지를 설치합니다.
npm install axios : 서버와 HTTP 통신을 하기 위한 라이브러리를 설치합니다.
npm install http-proxy-middleware : 개발 시에 CORS 문제를 방지하기 위해 프록시 설정을 도와주는 미들웨어를 설치합니다.
npm install @emotion/css, @emotion/react, @emotion/styled : CSS-in-JS 라이브러리인 Emotion 패키지를 설치합니다.
## 서버(Server)
npm init -y : 현재 디렉토리에 Node.js 프로젝트를 초기화합니다.
npm install express --save : Node.js에서 웹 서버를 구축하기 위한 Express 패키지를 설치합니다.
npm install nodemon --save : 개발 시에 파일 변경을 감지하고 서버를 자동으로 재시작해주는 Nodemon 패키지를 설치합니다.
npm install path --save : Node.js 내장 모듈인 path를 사용하여 파일 경로를 쉽게 다룰 수 있게 합니다.
npm install mongoose --save : MongoDB 데이터베이스와 연동하기 위한 Mongoose 패키지를 설치합니다.
MongoDB
MongoDB Atlas를 사용하여 클라우드에 MongoDB를 호스팅합니다. 본인의 계정으로 로그인하고 새 클러스터를 생성합니다.

## Express 앱 구축
Express 앱을 구축하고, 루트 경로에 대한 GET 요청에 "Hello World"를 응답하는 기본 서버를 설정합니다.

## MongoDB 스키마 생성
Mongoose를 사용하여 MongoDB 데이터베이스에 저장할 'Post' 모델을 정의합니다. postSchema에는 post의 'name'과 'content' 필드를 정의합니다.

## Proxy 설정
개발 환경에서 클라이언트와 서버가 다른 포트에서 실행될 때 발생할 수 있는 CORS 문제를 해결하기 위해 프록시 설정을 합니다. 클라이언트에서 '/api'로 시작하는 요청은 'http://localhost:5050'으로 전달됩니다. 이 설정은 클라이언트의 src 폴더에 setupProxy.js 파일을 생성하여 적용합니다.



## client
```
npx create-react-app .  
npm install react-bootstrap bootstrap
npm install react-router-dom   
npm install axios  
npm install http-proxy-middleware  
npm install @emotion/css
npm install @emotion/react
npm install @emotion/styled
```
## server
```
npm init -y;  
npm install express --save;  
npm install nodemon --save; 
npm install path --save;  
npm install mongoose --save;  
```

## monggodb
mongodb+srv://hoho:dlwm5656@cluster0.ctgdo3h.mongodb.net/?retryWrites=true&w=majority  


#### 터미널로 파일생성
echo "" > readme.md

#### 제작과정

```js
const express = require("express");
const app = express();
const port = 5050;

app.listen(port, () => {
    console.log("running --> " + port);
})

app.get("/", (req, res) => {
    res.send("Hello World")
})
```
## 서버 세팅

package.json 
```
test-> "start": "nodemon index.js"  
```

## http-proxy-middleware


미들 웨어..?

## </React.StrictMode>


## LF
git config --global core.autocrlf true



## __dirname

require
static


## 리액트 

https://cloud.mongodb.com
https://mongoosejs.com/


https://react-bootstrap.netlify.app 부트스트랩 react
https://emotion.sh  
https://tailwindcss.com/


https://axios-http.com/kr/docs/intro


app.use(express.static(path.join(__dirname, "../client/build/")));
app.use(express.json());
app.use(express.urlencoded({ extended: true }));



## MongoDB post 스키마 생성
```
const mongoose = require("mongoose");

const postSchema = new mongoose.Schema({
    name: String,
    content: String
})

const Post = mongoose.model("Post", postSchema);

module.exports = { Post };
```
Mongoose를 사용하여 MongoDB 데이터베이스에 저장할 'Post'라는 이름의 모델을 정의하는 코드입니다.

Mongoose는 MongoDB와 Node.js 사이의 객체 데이터 모델링(ODM) 라이브러리입니다. 이 라이브러리를 사용하면 MongoDB 데이터베이스에 저장할 데이터의 구조를 스키마로 정의하고, 이 스키마에 기반한 모델을 만들어 데이터베이스와의 상호작용을 쉽게 할 수 있습니다.

## 글 작성하기

https://reactrouter.com/en/main/hooks/use-navigate##usenavigate


## axios  
요청 req

## proxy 설정
루트 src폴더에 setupProxy 
middleware
"http-proxy-middleware": "^2.0.6", 설치 확인
```
const { createProxyMiddleware } = require('http-proxy-middleware');

module.exports = function (app) {
    app.use(
        '/api',
        createProxyMiddleware({
            target: 'http://localhost:5050',
            changeOrigin: true,
        })
    );
};
```
## 서버 index.js 기본 설정
```
const express = require('express')
const path = require("path")
const mongoose = require("mongoose")

const app = express();
const port = 5050;

app.use(express.static(path.join(__dirname, "../client/build")))

app.listen(port, () => {
    mongoose.connect(
        "mongodb+srv://hoho:dlwm5656@cluster0.ctgdo3h.mongodb.net/?retryWrites=true&w=majority"
    )
        .then(() => {
            console.log("connect --> " + port);
        })
        .catch((err) => {
            console.log(err)
        })
})
```
## react build 파일을 경로로 지정
```
app.get("/", (req, res) => {
    res.sendFile(path.join(__dirname), "../client/build/index.html")
})

app.get("*", (req, res) => {
    res.sendFile(path.join(__dirname), "../client/build/index.html")
})
```

## 서버로 요청
```
  axios.post("/api/test")
            .then((response) => {
                alert("요청 성공");
                console.log(response);
                setText(response.data.text);
            })
            .catch((err) => {
                alert("요청 실패");
                console.log(err)
            })
    }, [])
```
## 서버에서 요청 받고 보내줌
```
app.post("/api/test", (req, res) => {
    console.log(req);
    res.status(200).json({ success: true, text: "안녕하세요!" });
})
```


## 클라이언트에서 body[] 전송 
server index.js
body path 추가해야됨
```
app.use(express.json());
app.use(express.urlencoded({ extended: true }));
```


## 스키마 생성
```
const mongoose = require("mongoose");

const postSchema = new mongoose.Schema({
    name: String,
    content: String
}, { collection: "posts" })

const Post = mongoose.model("Post", postSchema);

module.exports = { Post };
```

## 스키마 생성, 데이터베이스에 데이터 저장
```
const { Post } = require("./Model/Post.js");


app.post("/api/test", (req, res) => {
    const BlogPost = new Post({ title: "안녕하세요", content: "내용입니다." })
    BlogPost.save().then(() => {
        res.status(200).json({ success: true });
    })
})

```

## 클라이언트 데이터 보내기
버튼 눌렀을떄 title content 보내기
```
const onSubmit = (e) => {
        e.preventDefault();

        if (title === "" || content === "") {
            return alert("내용을 채워주세요!")
        }
        let body = {
            title: title,
            content: content
        }
        axios
            .post("/api/post/submit", body)
            .then((res) => {
                if (Response.data.success) {
                    alert("글 작성이 완료되었습니다.");
                } else {
                    alert("글 작성이 실패하였습니다.")
                }
            })
    }
```

## 서버 데이터 받기 dm저장
```
app.post("/api/post/submit", (req, res) => {
    let temp = req.body;
    console.log(temp)


    const BlogPost = new Post(temp)
    BlogPost.save()
        .then(() => {
            res.status(200).json({ success: true });
        })
        .catch((err) => {
            res.status(400).json({ success: false })
        })
})
```

## LIST


클라이언트  

요청 성공시 포스트 리스트 받음
```
    const [postList, setPostList] = useState([]);

    useEffect(() => {
        axios.post("/api/post/list")
            .then((response) => {
                if (response.data.success) {
                    setPostList([...response.data.postList]);
                }
            })
            .catch((err) => {
                console.log(err)
            })
    }, [])
```


서버  

요청받으면 경로에 대한 post요청을 처리,
콜백함수 실행
.then((doc) => {...}) : find().exec()에서 반환받은 Promise가 resolve(성공) 되면 실행되는 콜백 함수
찾아낸 문서들이 doc에 담겨서 전달
이 콜백 함수 내부에서는 res.status(200).json({ success: true, postList: doc })를 통해 HTTP 상태 코드 200과 함께 성공 메시지와 찾아낸 문서들을 JSON 형태로 응답
```
app.post("/api/post/list", (req, res) => {
    Post.find().exec()
        .then((doc) => {
            res.status(200).json({ success: true, postList: doc })
        })
        .catch((err) => {
            console.log(err)
            res.status(400).json({ success: false })

        })
})
```
find 찾기
exec 실행
찾아서 실행



## 게시물 PostNum 생성시키기
-번호 1씩 증가시켜서 저장 (게시글 수정, 삭제시 필요함)

### 1. Counter 스키마 생성
```
const mongoose = require("mongoose");

const counterSchema = new mongoose.Schema({
    name: String,
    postNum: Number
}, { collection: "counter" })

const Counter = mongoose.model("Counter", counterSchema);

module.exports = { Counter };
```
```
const { Counter } = require("./Model/Counter.js");
```
### 2. 번호 1씩 증가시켜서 저장
-{ $inc: { postNum: 1 } } 증가시키기
```
app.post("/api/post/submit", (req, res) => {
    let temp = req.body;
    // 넘버 추가 작업 (글 삭제,수정하기위해)
    Counter.findOne({ name: "counter" })
        .exec()
        .then((counter) => {
            temp.postNum = counter.postNum;

            const BlogPost = new Post(temp);

            BlogPost.save()
                .then(() => {
                    // 번호를 1씩 증가
                    Counter.updateOne({ name: "counter" }, { $inc: { postNum: 1 } })
                        .then(() => {
                            res.status(200).json({ success: true });
                        })
                })

        })
        .catch((err) => {
            console.log(err)
            res.status(400).json({ success: false })
        })



    const BlogPost = new Post(temp)
    BlogPost.save()
        .then(() => {
            res.status(200).json({ success: true });
        })
        .catch((err) => {
            console.log(err)
            res.status(400).json({ success: false })
        })
})
```
