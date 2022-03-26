#Class_Arrangement
# CodeVita_2022
![WhatsApp Image 2022-03-26 at 12 00 11 PM](https://user-images.githubusercontent.com/43782542/160235277-de70dac1-d063-4481-b4ed-9f1c5e4936a9.jpeg)



    ls=['G','G','B','B','G']
    n=len(ls)
    def swap(P,Q):
        temp_1 = ls[P]
        ls[P] = ls[Q]  
        ls[Q] = temp_1 
        print(ls)
    for i in range(n-1):
        if ls[i]!=ls[i+1]:
            continue
        else:
            k=i+1
            step=0
            for j in range(k+1,n):
        
                if ls[k]!=ls[j]:
                    if step==0:
                        print(ls)
                        swap(k,j)
                        print(k,j)
                        break
                    else:
                        print('s')
                        step= step-1
                else:
                    if ls[k]== ls[j]:
                        print('step')
                        step= step+1
               
