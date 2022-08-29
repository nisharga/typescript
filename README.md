************** TypeScript Vs es6 *****************************<br>
everything is same to same, but only difference is ":string" this line.
let student: string = 'nisharga';
when we use es6, we use let student = 'nisharga';
but in typeScript.... let student: string = 'nisharga';

let age: number = 10;
let isSmart: boolean = false;

let presedent: string[] = ['jho', 'baidan', 'Love', 'hope'];
let numbers: number[] = [1, 2, 3];

when object or array this type of things happen.....

const person: {name: string, age: number, job: string} = {
  name: "Nisharga",
  age: 20,
  job: 'kaj nai'
}

then smartest method this is......................<br>
<code>
interface Kaj{
  title: string;
  bill: number;
  suti: boolean;
}
const kaj: Kaj ={
  title: "Boss",
  bill: 2200,
  suti : false,
}
</code>



**************** using UseState **********************
<code>
interface User{
  name: string;
  job: string;
}

const [user, setUser] = useState<User | null>(null);
const handleIncrise = (): void=>  {
    setCounter(counter + 1);
  }
  
const handleUserSubmit = (e : any) => {
    e.preventDefault();
    const userdata = {
      name: "Nisharga",
      job: "Bekar",
    }
    setUser(userdata);
  }
  
<button onClick={handleUserSubmit}>Add User</button> 
</code>


************************ Using Props ******************
<code>
<Person name="Nisharga" age={22}></Person> (HOMEPAGE)

const Person = ({name, age}: {
    name: any;
    age: any;
}) => {
	return(
<h2>Person name is {name} and age is {age}</h2>
);
}

<bold>Alternative option</bold>
interface Props{
    name: string;
    age: number;
}
const Person: FC<Props> = ({name, age}) => {}
</code>





<b>************* Clone a repo from Github and upload it on own github ************************* </b>
<code>git clone --bare</code> (git link) Clone a repo with commit and all those things
after that go to git folder like this......... cd folderName.git
Then create a new Repo on GitHub && collect the NewGitLink
after that command this............ git push mirror NewGitLink.git


<b>************* Local folder github upload repo change origin *************************</b>
If already in Local Folder, Already file upload in a git repo. But you want to change .git location
first check in that folder by this comand... <code>git remote -v </code>
then collect the new origin && comand here....... <code>git remote set-url origin newOrigin.git</code>
then again check the origin.......... <code>git remote -v </code>
