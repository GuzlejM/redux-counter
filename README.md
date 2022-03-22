1. Create store folder
2. Inside store folder Create reducers folder
3. <name>Reducer.js holds the state lets create reducer
4. Create index.js inside reducers folder, Import combineReducers function and call it with object <name> : <name>Reducer
5. Create store.js inside store folder createStore() function and export it out to store
6. Import { Provider } Into index.js from react-redux and WRAP the app with the <Provider></Provider>
7. Import { store } from store and pass store as prop to <Provider store={store}></Provider>
8. How to access store ? SPECIAL HOOK from Redux
9. { useSelector } from react-redux
10. Under the App() const state = useSelector((state) => state);
11. Create action-creators with index.js inside of Store folder
12. Create function deposit money with amount parameter and return (dispatch)
13. index.js inside store put in export \* as actionCreators from "./action-creators/index";
14. Inide App.js { useDispatch } from actionCreators same as useSelector
15. Inide App.js { bindActionCreators } from redux
16. Inide App.js { actionCreators } from store/index.js
17. Inide App.js const AC = bindActionCreators(actionCreators, dispatch);
18. store.js needs:

import { createStore, applyMiddleware } from "redux";
import thunk from "redux-thunk";
const store = createStore(reducers, {}, applyMiddleware(thunk));

19.
# redux-counter
