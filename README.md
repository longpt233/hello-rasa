## hello-rasa
test thử venv và rasa


## rasa command

```
rasa init 
rasa train 
rasa shell 
rasa run --enable-api 
rasa run actions 
```

## how to use venv 

- create env
```
python -m venv venv

```
- select env (ctrl + shift +p )  
- new terminal 
- install: 
```
pip install -r requirements.txt
```

## how to create 

- in nlu.yml :example -> intent. điền vào intent + example . có thể dùng lockup để thêm nhiều từ cho một ngữ cảnh -> để học tốt hơn 
- in rules.yml :intent-> action. điền vào action tương ứng với intent bên trên 
- in domain.yml :
  -  định nghĩa lại intent vô đây   
  -  dinh nghia action-> return ngay text : response . pre = utter.       
  -  định nghĩa action-> more action      : action   . pre = action. tên này trùng với tên trong action.py    


## note : 
- khi nào nên dùng action : 
  - bthg dùng rasa như tách từ call service.    
  - khi cần xử lí các tác vụ liền mạch, lưu tracking, session 

- rasa nlu, rasa core 
- story.yml để có ngữ cảnh hơn là chỉ hỏi đáp 
- thêm action thì nhớ mở cổng 5055 trong file nào ấy 
- muon extract entity thi dung symptom, add trong nlu + domain>slot
- nen lay cac cau train trong nlu co entity sample khac nhau new york-Los Angeles,... vi mac du co lockup nhung no k work lam 
