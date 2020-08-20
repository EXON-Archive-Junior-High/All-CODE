# Eat
```cs
Food food = new Food("Chicken");
Time t = new Time("5h");
food.ToMouth().Digest(t);
```
# Class
## Food
### Food(string foodName)
foodName이란 이름의 음식 선언
### ToMouth() : DigestibleFood
입에 넣기 <br>
DigestibleFood 객체 반환.
## Time
### Time(string time)
## DigestibleFood
### Digest(Time time)
DisgestibleFood 객체를 time의 시간동안 소화시킵니다.
