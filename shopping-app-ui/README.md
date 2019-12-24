COMMANDS SECTION : 
this section about the commands that has been used in this application and why
1- expo int application-name
create new expo or react native project in the specified location you choose some defult options 
2- npm install --save redux react-redux react-navigation react-navigation-header-buttons

react-naviation: for navigation services.
redux : for state management
react-navigation-header-buttons : This will add header buttons and we want to have these nicely styled and positioned buttons without having to do all that styling positioning on my own.

3- expo install React-native-gesture-handler react-native-reanimated
4- install the following libs for navigation:
    1- npm install --save react-navigation-stack
    import { createStackNavigator } from 'react-navigation-stack';

    2- npm install --save react-navigation-tabs
    import { createBottomTabNavigator } from 'react-navigation-tabs';

    3- npm install --save react-navigation-drawer
    import { createDrawerNavigator } from 'react-navigation-drawer';


PLANNING SECTION : 
1- Lec 157 for planning to that project and what screens we need and the purpose of this screen
2- Lec 158 create baisc project setup and also create folders structure :
    2.1- components 
    2.2- constants
    2.3- navigation
    2.4- screens 
            -> shop ->ProductOverviewScreen.js
            -> shop ->ProductDetailsScreen.js
            -> shop ->CartScreen.js
            -> shop ->OrderScreen.js

            -> user ->UserProductScreen.js
            -> user ->EditProductScreen.js

            -> store
3- Lec 159 The Products Overview Screen : The goal is to present a list of all the products we can order ,here we will create the baisc content of this  screen and also models for the product inside models folder.
also add actions and reducers folders inside the store folder for redux to manage the state
also setup dummay data.

in App.js we need to import the createStore,combinedReducers and Providers and then create the root reducer and also make the Provider HOC wrap-up the App.js export part

4- Lec 160 Setting Up a Navigator : useSelector used here to read from redux.setting up the navigation in the shopNavigator.js here is the stackNavigation with [screens and navigation default options] should be defined and options are added




