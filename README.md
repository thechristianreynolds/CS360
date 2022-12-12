# CS360

---

#### Project Goals

The goal of this project was to create an inventory application. This application was designed to allow users to store item inventory with an Android application. This included persistent data, the ability to add new items, the ability to update item quantities, and the option to receive low stock notifications for a particular item.

#### User Interface

The main screens of this app are listed here:
| Screen    | Purpose |
| ----------- | ----------- |
| Login     | Allow a user to login with an existing account or register a new account        |
| ViewDatabase   | Allow a logged in user to see a visual representation of their inventory items, update select item quantities, and view a menu with options to add a new entry or view the settings screen.|
|AddNewEntry| Allow a logged in user to add a new item to their database with required fields **Item Name** and **Item Quantity** |
| Settings | Allow a logged in user to change app notification behavior **on** or **off** |

#### Implementation

I started the development process by taking the user requirements and translating them into high level comments or pseudocode. This gave me a solid outline or framework to work towards a completed application. From here, I followed a process of implementing the commented code, breaking the commented code into more specific sections, implementing the more specific comments, and repeating this process for almost every aspect of the completed application. The advantage of this approach is that the development process produces nice documentation and code comments.

#### Testing

To ensure application functionality, I manually tested each requirement on three separate SDK targets. Since this application only had a few major requirements, each one could be tested manually without consuming too much time. I testing this app on the latest SDK and the two before it with an emulator, and again tested the app on the latest SDK on a physical device. 

#### Challenges

The most difficult part for me was the notification permissions process. It was hard to test if the user would be prompted for this permission because after the first run, the prompt would no longer show up. I worked this out by creating a nice function that tells if it's the first time the application has been run, and this value is used to determine if a prompt should be shown to the user. This prompt shows up every time application data is cleared.

#### Success

The ViewDatabase screen shows off a lot of my knowledge and skills as a developer. It includes CRUD functionality with a persistent database, the use of an Android recycler view, and the use of java interfaces. 