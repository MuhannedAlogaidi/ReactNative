1- Create the project and install it => npm install
2- Create essentials folders 
    2.1- Components 
    2.2- Screens : we have the very basic setup we need here, though of course all our screens are totally empty
        2.2.1 : Categories Screen and I'll name the file categories screen to make it really clear what's inside there. This is the screen where we can select a category like Italian, German, American, so where we can select a food category.
        2.2.2 : Category Meals Screen we will see a list of meals that fits into this category.this is the screen that loads the meals for a chosen category.
        2.2.3 : Favorites Screen which is the screen that holds all our favorite recipes, our favorite meals.
        2.2.4 : MealDetailScreen, that's the screen we see if we tap on a single meal inside of a chosen category or on the favorite screen. This then shows us the ingredients and the detailed steps for this meal.
        2.2.5 : Filters Screen and this filters screen is the screen that allows us to set filters, like vegan food so that we only see recipes which are vegan or vegetarian or glutenFree or lactoseFree.
3- Add Fonts : how to expo fonts and how to install,fetch and use .
    3.1 : Install expo-font via npm install expo-font --save
    3.2 : Import fonts from expo fonts [ see app.js ]
    3.3 : Import the AppLoading component from expo, that's the component that will prolong the splash screen when the app starts until our fonts are loaded so that we only see something on the screen when all our assets, and in this case these are the fonts, are really available and are really there.
    3.4 : Create an object that fetch or hold the fonts as an key value by using function called LoadAsync and return promise. Then use conditionally <AppLoading> component that load the application in case of the font are loaded as well as all assests, see the condition   if (!fontLoaded) { ... 
4- Installing React Navigation & Adding Navigation to the App
    4.1- Install React navigation via npm install --save react-navigation and also install these dependencies 
    expo install react-native-gesture-handler react-native-reanimated
    4.2- Create folder Called Navigation and inside it create file called MealsNavigator.js
    4.3- while we are using ReactNavigation v4 , then install the following :
        4.3.1- createStackNavigator : objects, actually React components as it will turn out, which hold all the navigation configuration, which hold all the information which different screens you have and which will do the heavy lifting of loading different screens and playing nice smooth transitions for going from A to B for you.
        npm install --save react-navigation-stack and import { createStackNavigator } from 'react-navigation-stack';
        4.3.2- wrap the createStackNavigator by createAppContainer and import it import { createAppContainer } from 'react-navigation';
        Notice : createStackNavigator it is a function that take an object . this object hold Key/Value. key can be object that hold the screen path (component) and other data
5- Navigate between screens: here are multiple things either FIFO i mean stact , it means navigate throught one way and return back same way.
PUSH , POP and replace are another way to navigate between screens . PUSH and POP add one screen rout or remove from the top but the syntax will be diffrent little bit 

6- Grid and Columns with navigation and dymmay data and style it
7- Configuring the Header with Navigation Options , it is a special props that used to give the screen or navigation an additional propterties

8- Passing & Reading Params Upon Navigation : passing param you can add it as a second param to props.navigation.navigate function. see this line  props.navigation.navigate({
            routeName: 'CategoryMeals',
            params: {
              categoryId: itemData.item.id
            }
});
an also on the landing page should read the param that comes with the navigation or from , see this line :
  const catId = props.navigation.getParam('categoryId');
8- Read the default options for navigation for            


