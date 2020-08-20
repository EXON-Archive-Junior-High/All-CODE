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
Git git = new Git();
git.Commit("코딩 이제 안한다");
git.Push();
```
## Computer

### <b>Function</b>
### Computer(string cpu, string gpu, string ram)
cpum gpu, ram 사양인 컴퓨터 생성

### Start
Computer 객체를 시작한다.

### Program FindProgram(string programName)
Computer 개체에 programName의 이름을 가진 Program 객체를 반환한다.

### <b>Field</b>
### bool isStarted
Computer 객체가 시작되었는지

## Program
### <b>Function</b>

### 
