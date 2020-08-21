# Coding
```cs
Computer com = new Computer("i9-990kf", "GTX 1650", "32GB");
if (!com.isStarted) com.Start();
Program vsc = com.FindProgram("Visual Studio Code");
if (vsc.name == string.Empty) return "vsc 깔고 와";
vsc.Start();
Idea idea = new Idea("GoodIdea");
Brain br = new Brain("GoodBrain");
br.TalkToBrain($"{idea.content}이 아이디어를 개발해!");
while (true){
    br.TalkToBrain("개발해");
    if (br.programIsComtlete) break;
    if (br.isDead) return "삼가 고인의 명복을..";
}
br.TalktoBrain("Good Job");
vsc.Save();
Git git = new Git(vsc);
git.Commit("코딩 이제 안한다");
git.Push();
vsc.Stop();
```
## Computer

<b>Function</b>

### Computer(string cpu, string gpu, string ram)
cpum gpu, ram 사양인 컴퓨터 생성

### Start
Computer 객체를 시작한다.

### Program FindProgram(string programName)
Computer 개체에 programName의 이름을 가진 Program 객체를 반환한다.

<b>Field</b>
### bool isStarted
Computer 객체가 시작되었는지

## Program
<b>Function</b>

### void Start()
Program 객체를 실행합니다.

### void Stop()
Program 객체를 중단합니다.

### void Save()
Program 객체에 대한 내용을 저장합니다.

<b>Field</b>

### string name
Program 객체의 이름

## Idea
<b>Function</b>

### Idea(string ideaType)
ideaType 에 맞는 아이디어를 생성합니다.

<b>Field</b>

### string content
Idea 객체의 내용입니다.

## Brain

<b>Function</b>

### Brain(string brType)
brType 에 맞는 브레인 모델을 생성합니다.

### void TalkToBrain(string content)
content 를 브레인 모델에게 전달(말)합니다. <br>
또한 브레인 모델에게 전달한 것으로 브레인 모델이 실행됩니다.

<b>Field</b>

### bool programIsComtlete
브레인 모델이 프로그래밍을 종료했는지에 대한 필드입니다.

### bool isDead
브레인 모델이 죽었는지에 대한 필드입니다.

## Git

<b>Function</b>

### Git()
새로운 Git 객체를 생성합니다.

### void Commit(Program vsc)
vsc 에 변경된 내용을 Git 객체에 커밋합니다.

### void Push()
Git 객체를 Push 합니다.

