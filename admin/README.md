## Admin 바뀐점

기존? => [admin](https://github.com/BH946/fullstack-clone/tree/shop-cart-admin) 들어가서 확인

바뀐점들 자세히 보고싶다면, 커밋내용 확인할 것

추가된 파일들만 따로 정리하겠다.

<br>

## Folder Structure - 추가된 점

* [setupProxy.js](/client/src/setupProxy.js)
  * cors(크로스 브라우징) 문제 해결
* [requestMethods.js](/client/src/requestMethods.js)
  * api 호출 axios.create하는 부분
  * 여기서 로컬에 저장된 TOKEN 또한 가져와서 headers에 추가해서 api 요청을 하게된다.

* [firebase.js](/admin/src/firebase.js)
  * 이미지를 firebase에 추가하며 응답으로 얻은 이미지 저장된 URL을 가져와서
  * 몽고DB에 저장해서 이를 활용해서 제품들을 추가한다.
* [Login.jsx](/admin/src/pages/login/Login.jsx)
  * 로그인 기능을 추가
* [apiCalls.js](/admin/src/redux/apiCalls.js)
  * api 호출과 Redux와 연동해서 CRUD 형성
* [productRedux.js](/admin/src/redux/productRedux.js)
  * api 호출과 Redux와 연동해서 CRUD 형성
* [store.js](/admin/src/redux/store.js)
  * Redux 활용할때 실제로 사용되는 파일
  * persist를 활용
* [userRedux.js](/admin/src/redux/userRedux.js)
  * api 호출과 Redux와 연동해서 로그인 기능정도만 형성