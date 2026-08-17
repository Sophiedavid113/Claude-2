1:    React Component
   file extension:  react file ka name jsx  ho ga
............................
   function component : function app( ) {
 return <H1> header <H1>    } 
export default app:
.............................
Type of export component 
Default component:   ek file me aik ki default export ho Sakta hia
............................
Named component: me multiple name export ho sakte Han.
............................
2:  Jsx : app.js se Jo code likhta hu wo html Nahi Javascript hia.
............................






<>      <H1> 1234</H1>      </>
<React.Fragment>    <H3> 1234 </H3>
</React.Fragment>
....................................fragment.................
Let Students =["Hamza","Bilal"];
{students.map((student)  = > 
(<H2> {student} </H2> 
}));
array.map((item, index) => (
  <JSX />                syntax
));
.........................................map method......
function app ( ) {const is login = true;
if( login) {   return  <H1>123</H1>;
} else {return <H1>456</H1>;      }


if (condition) { 
  return (
    // True ہونے پر یہ JSX چلے گا
  );
} else {
  return (
    // False ہونے پر یہ JSX چلے گا
  );
}
 
.


.......conditional rendering if else method
const add = true;    return ( <div> {add && <H1>123<H1> }):} </div>
{
  condition && <JSX />     syntax
}
......conditional rendering  and method..

اگر شرط (Condition) true ہو تو اس کے بعد والا JSX یا Component دکھاؤ، اور اگر شرط false ہو تو کچھ بھی نہ دکھ        if
 
اگر condition true ہو → JSX نظر آئے گا۔
اگر condition false ہو → کچھ بھی نظر نہیں آئے گا۔                                and  





function App() {
  const names = ["Ali", "Ahmed", "Sara"];
  return (
    <div>
      {names.map(name => (
        <p>{name}</p>
      ))}
    </div>
  );
}
............................. lists...........................







.function Profile(props) {
  return <img src={props.image} alt="profile" />;
}
<Profile image="photo.jpg" />
.................................................props..........
function Card(props) {
  return <div>{props.children}</div>;
}
<Card>
  <h1>Welcome</h1>
</Card>
..................................children props.........

آسان تعریف: Props وہ طریقہ ہے جس کے ذریعے Parent Component اپنے Child Component کو data بھیجتا ہے۔.








<Link to="/about">About</Link>
Page reload kiye bagair     01    to
 
Page Reload کیے بغیر دوسرے Page پر لے جاتا
 ہے۔ <Link to="/about">About</Link>  
                                              02   Link

<Route path="/" element={<Home />} />       element وہ پراپرٹی ہے جو بتاتی ہے کہ کسی خاص URL پر کون سا React Component یا Page دکھانا ہے۔              element   03

path="/about"               04 path.
............................react router 01....




 یہ ایک URL اور ایک Component کو آپس میں جوڑتا ہے۔. <Route path="/"  element={<Home />} />    
Route 05......................................................
    اس کے اندر تمام Routes لکھے جاتے ہیں
   Routes>

        <Route path="/" element={<Home />} />
<Route path="/about" element={<About />} />
  </Routes>
 Routes 06..................................................
..
BrowserRouter براؤزر کا راستہ (URL) دیکھتا ہے اور اس کے مطابق React کا صحیح Page کھولتا 
Browserrouter 07........................................
...................react router 02.......


function App() {
0  return (
    <button onClick={() => alert("Button Click Hua!")}>
      Click Me
    </button>       );
.............................onClick event handling
function handleClick() {
  alert("Button Click Hua!");
}
...........................onClick event handling...

.....................................................................
<button onClick={handleClick}>Click Me</button>       syntax   

.................... event...............................
........


Mounting
جب Component پہلی بار Screen پر آتا ہے تو اسے Mounting کہتے ہیں۔
Component بنتا ہے۔
JSX Render ہوتا ہے۔
Screen پر نظر آتا ہے۔
..................................................................
Updating 
جب State یا Props تبدیل ہوں تو Component دوبارہ Render ہوتا ہے، اسے Updating کہتے ہیں۔
Component دوبارہ Render ہوتا ہے۔
Button پر Click کیا۔
Count 0 سے 1 ہو گیا۔
.....................................................................
unmounting 
جب Component Screen سے ہٹا دیا جائے تو اسے Unmounting کہتے ہیں۔
Component ختم ہو جاتا ہے۔
Memory صاف کی جاتی ہے۔
اگر Timer یا Event لگا ہو تو اسے بھی ختم کیا جاتا ہے۔
مثال:
Home Page سے About Page پر چلے گئے۔
Home Component Screen سے ہٹ گیا۔

............................. mounting......


..usestate react Ka ik hook hia Jo data KO store or update krne ke liye istamal hota
¹aimport { useState } from "react";

function App() {
  const [count, setCount] = useState(0);
  return (
    <>~
      <h2>Count: {count}</h2>
      <button onClick={() => setCount(count + 1)}>
        Increase
      </button>
    </>
  );
}
export default App;




useState React کا ایک Hook ہے جو Functional Component کے اندر State (ڈیٹا) کو بنانے اور اپڈیٹ کرنے کے لیے استعمال ہوتا




.....................use state hook...........





..Yani component render hone ke baad useEffect apna kaam karta hai. component render console.log me print ho ga 
useEffect(() => {
  console.log("Page Load");
}, []);        
..................................... useEffect hook......


...useContext = Ek jagah data rakho aur jis component ko zarurat ho, woh wahin se data le le.      example internet = data
Mobile TV laptop = component
// Profile.js

import { useContext } from "react";
import { ImageContext } from "./ImageContext";

function Profile() {
  const image = useContext(ImageContext);
  return (
    <div>
      <h2>User Profile</h2>
      <img
        src={image}
        alt="Profile"
        width="200"
      />
    </div>
  );
}
export default Profile;

useContext(ImageContext); 

//Data lena//
Create context     context banana hia
userContext      UserContext = Data share karne ka container (dabba) ya system hai.

.....................................................................
............................ useContext hook...........









..........









