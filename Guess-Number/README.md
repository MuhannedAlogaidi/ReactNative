## GUSS A NUMBER app

### source is Maxi from UDAMY Section 4: Components, Styling, Layouts - Building Real Apps

build an application where I want to have a little header at the top, so a little bar at the top which simply displays the title which is guess a number because we'll build an application where you enter a number and the app will try to guess it.

we'll have a starting screen where you have an input for your number which the user of the app can enter and then of course, we'll have two buttons, basically a confirm button here and a reset button here, so two buttons that allow us to control that input, then a button to basically start the game.

so once you chose a number which basically loads a different screen you could say which still has our title at the top but where now the computer will output I guess let's say 63 initially, so that's guess from the computer which you kind of output in a nicer way here and then you have to tell whether the actual number is lower or greater than what the computer guess here, so you've got two buttons to control this.

We want to show an alert if you give the user a wrong hint, so if your number is lower and you say greater, then I want to show an alert where we say something like don't cheat, anything like that, so little check in there and once the computer guessed the right number,

so once the game is over basically, we'll have a game over screen here where we say something like gameover, where I then want to output an image here, maybe such a rounded image like some goal image, a summit, something like this and below that, we'll output some info text like the computer guessed your number 15 in 10 guesses.

So basically a summary and also a button to basically restart and play a new round with a new number. 

<div style="text-align: right"> So the nice thing about this application is that whilst it of course isn't overly complex, there aren't tens of dozens of screens involved but whilst that is the case, we have a lot of different components which we also can style and layout, we use an image, we'll use our own custom fonts and we have also quite a bit of business logic in there to control the guessing, to check whether the correct number was guessed and so on. So it's a really nice app, a real nice second step which will make sure that all the basics are super clear and set after this module so that you are more than well-prepared for more advanced applications after this great application here. </div>

### Implementation
#### Step 1 : Create the container may be the app.js as an empty component .
#### Step 2 : Create the Headr.js component . prepare the style and contnets
          #### Step 2.1 : create shadow for card
#### Step 3 : Create the Screen.js component . prepare the style and contnets
#### Step 4 : Build first reuse component which is the shadow card will act like container . pay attention to this code for object distrubutiona see the props.children
> ```javascript
> <View style={{ ...styles.card, ...props.style }}>{props.children}</View>
> ```
#### Step 5 : Build a reuse input component, notice the porps and style same as point 4.
          ### Step 5.1 : Import the input to Screen.js component , add the event to handle the input changes
          ### Step 5.2 : Use TouchableWithoutFeedback the touchable without feedback component, so a component that allows us to
          gister a touch listener without giving any visual feedback because. on there, we can now register or listen 
          to the press event and when a press happens, I want to dismiss the keyboard and for that, React Native gives 
          us a useful API we can import from React Native and that's the keyboard API. That's now not a component but                             that's an API where we can interact with the native device itself
                          

