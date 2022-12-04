************** TypeScript Vs es6 *****************************<br>
everything is same to same, but only difference is ":  string" this line.<br>
let student: string = 'nisharga';<br>
when we use es6, we use let student = 'nisharga';<br>
but in typeScript.... let student: string = 'nisharga';<br>

let age: number = 10;<br>
let isSmart: boolean = false;<br>

let presedent: string[] = ['jho', 'baidan', 'Love', 'hope'];<br>
let numbers: number[] = [1, 2, 3];<br>

when object or array this type of things happen.....<br>
<code>
const person: {name: string, age: number, job: string} = {<br>
  name: "Nisharga",<br>
  age: 20,<br>
  job: 'kaj nai'<br>
}<br>
</code>

then smartest method this is......................<br>

<code>
	
interface Kaj{ 
  title: string;<br 
  bill: number;<br> 
  suti: boolean;<br> 
}<br> 
const kaj: Kaj ={<br> 
  title: "Boss",<br>
  bill: 2200,<br><br> 
  suti : false,<br> 
}<br> 
	
</code>




**************** using UseState **********************<br>
<code>
interface User{<br>
  name: string;<br><br>
  job: string;<br>
}<br>

const [user, setUser] = useState<User | null>(null);<br>
const handleIncrise = (): void=>  {<br>
    setCounter(counter + 1);<br>
  }<br>
  
const handleUserSubmit = (e : any) => {<br>
    e.preventDefault();<br><br>
    const userdata = {<br>
      name: "Nisharga",<br><br>
      job: "Bekar",<br>
    }<br><br>
    setUser(userdata);<br>
  }<br>
  
<button onClick={handleUserSubmit}>Add User</button> <br>
</code>


************************ Using Props ******************<br>
<code>
<Person name="Nisharga" age={22}></Person> (HOMEPAGE)<br>

const Person = ({name, age}: {<br>
    name: any;<br>
    age: any;<br>
}) => {<br>
	return(<br>
<h2>Person name is {name} and age is {age}</h2><br>
);<br>
}<br>

<bold>Alternative option</bold><br>
interface Props{<br>
    name: string;<br>
    age: number;<br>
}<br>
const Person: FC<Props> = ({name, age}) => {}<br>
</code><br>





<b>************* Clone a repo from Github and upload it on own github ************************* </b><br>
<code>git clone --bare</code> (git link) Clone a repo with commit and all those things<br>
after that go to git folder like this......... <code>cd folderName.git</code><br>
Then create a new Repo on GitHub && collect the NewGitLink<br>
after that command this............ <code>git push mirror NewGitLink.git</code><br><br>


<b>************* Local folder github upload repo change origin *************************</b><br>
If already in Local Folder, Already file upload in a git repo. But you want to change .git location<br>
first check in that folder by this comand... <code>git remote -v </code><br>
then collect the new origin && comand here....... <code>git remote set-url origin newOrigin.git</code><br>
then again check the origin.......... <code>git remote -v </code><br>
	
	
<b>************* Deploy FrontEnd in Vercel *************************</b><br>
Firstly you have to install in your PC via:  <code> <b> npm i -g vercel </b> </code> 
Secondly, Create an acccount on vercel.com.

#Vercel deploy</b><br>	
0.in cmd comand vercel (then login)</b><br>
1.Setup and deploy "address" - Y</b><br>
2.scope (Account name) - select that</b><br>
3.Link to existing project - N</b><br>
4.Whats your project name - Enter + Enter</b><br>
5.Want to modify these settings - N</b><br>

#Top Tip to get a job:
