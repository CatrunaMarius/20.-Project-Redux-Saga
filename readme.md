## 20.  Project Redux-Saga
Before we continue, I would like to make one quick correction about when Sagas fire in our redux flow.  I mentioned that sagas fire before reducers, it's actually the other way around! Reducers fire first, then sagas receive the action. From there, sagas can fire off new actions which in turn hit the reducers and other sagas as well!

This correction does not change any of the code we will write for the remainder of the course, it's just a small correction on a theoretical level. The impact is also not significant because we write actions that only our sagas are listening for, our reducers receiving it before the sagas is not an issue because our reducers are not reacting to these actions that are intended for our sagas

Keep in mind that getting redux-sagas in one go is usually impossible and it is something you practice multiple times to fully understand.

### Referince link
[Generator function documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function*)

[redux-saga npm](https://www.npmjs.com/package/redux-saga)

[What is Redux-Saga](https://engineering.universe.com/what-is-redux-saga-c1252fc2f4d1)

[Understanding redux-saga: From action creators to sagas](https://blog.logrocket.com/understanding-redux-saga-from-action-creators-to-sagas-2587298b5e71/)

[redux-saga.js.org](https://redux-saga.js.org/)