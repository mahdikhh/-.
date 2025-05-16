f = input ('txt ra bego :')
d={}
# شمارش تعداد تکرار کاراکترها
for i in f :
    d[i] = d.setdefault(i,0)+1
#بر اساس حروف الفبا به ترتیب نمایش میدهد
sorted = sorted(d.items() , key=lambda items: items[0] )
for k , v in sorted :
    
    print(f'tedad charekter {k} barabar {v} ast .')



'''برای اینکه بر اساس تعداد تکرار باشد بدین گونه میشود:
sorted = sorted(d.items(), key=lambda items: items[1], reverse=True)

for k , v in sorted :
    
    print(f'tedad charekter {k} barabar {v} ast .')'''
