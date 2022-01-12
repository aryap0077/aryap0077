from tkinter import *

#this specifies the size appearance and title of the output window
root=Tk()
root.geometry("1920x1080")
root.title("Industry Management")
photo=PhotoImage(file ="billing.jpg")
root.iconphoto(False, photo)
root.resizable(True,True)
#main title 
lbl=Label(font=('Agency FB',45,'bold'),text="Industry management system", bd=16).pack()
#defining function for exit button 
def exit():
    root.destroy()

#defined function for billing button    
def billing():
    #function for reset button
    def Reset():
        entry_Tshirt.delete(0,END)          #predefined function to clear the entries provided
        entry_Jeans.delete(0,END)
        entry_Shirt.delete(0,END)
        entry_Jacket.delete(0,END)
        entry_Mask.delete(0,END)
        entry_Cap.delete(0,END)
        entry_Shoes.delete(0,END)
        
    #function for total button
    def Total():
        try:a1=int(Tshirt.get())            #these get the input the user provides
        except:a1=0

        try:a2=int(Jeans.get())
        except:a2=0

        try:a3=int(Shirt.get())
        except:a3=0

        try:a4=int(Jacket.get())
        except:a4=0

        try:a5=int(Mask.get())
        except:a5=0

        try:a6=int(Cap.get())
        except:a6=0

        try:a7=int(Shoes.get())
        except:a7=0

      
        #defining cost of each item per quantity
        c1=800*a1
        c2=1600*a2
        c3=1000*a3
        c4=3000*a4
        c5=240*a5
        c6=450*a6
        c7=1300*a7


        labl_total=Label(f2,font=("Aria",21,"bold"),textvariable=Total_cost,bg="lightyellow")   #label for cost
        labl_total.place(x=0,y=100)

        Label_tax=Label(f2,font=("Aria",21,"bold"),textvariable=Total_tax,bg="lightyellow")     #label for tax
        Label_tax.place(x=0,y=150)
        
        lbl_total=Label(f2,font=("Aria",21,"bold"),textvariable=Total_bill,bg="lightyellow")    #label for total bill
        lbl_total.place(x=0,y=200)       

       
        totalcost=c1+c2+c3+c4+c5+c6+c7
        a_cost="Total..........Rs.",totalcost
        Total_cost.set(a_cost)                          #defined total cost text variable
        
        tax=(12/100)*totalcost
        tmp=int(tax)
        a_tax="12%GST....Rs.",tmp
        Total_tax.set(a_tax)                            #defined totaltax text variable
        
        totalamount=totalcost+tax
        a_bill="Inc.Tax......Rs.",totalamount
        Total_bill.set(a_bill)                          #defined totalbill text variable

        
    Label(text="Bill Management",bg="black",fg="white",font=("Agency FB",30),width=105,height=2).place(x=0,y=230) #label for bill title

    #List of item
    f=Frame(root,bg="skyblue",highlightbackground="black",highlightthickness=1,width=300,height=420)    #frame added for list of items
    f.place(x=180,y=345)
    #labels for different items available
    Label(f,text="List of item",font=("Gabriola",40,"bold"),fg="black",bg="skyblue").place(x=50,y=0)
    Label(f,font=("Arial",20,'bold'),text="T-shirt.....Rs.800",fg="black",bg="skyblue").place(x=10,y=80)
    Label(f,font=("Arial",20,'bold'),text="Jeans.....Rs.1600",fg="black",bg="skyblue").place(x=10,y=120)
    Label(f,font=("Arial",20,'bold'),text="Shirt.....Rs.1000",fg="black",bg="skyblue").place(x=10,y=160)
    Label(f,font=("Arial",20,'bold'),text="Jacket.....Rs.3000",fg="black",bg="skyblue").place(x=10,y=200)
    Label(f,font=("Arial",20,'bold'),text="Mask.....Rs.240",fg="black",bg="skyblue").place(x=10,y=240)
    Label(f,font=("Arial",20,'bold'),text="Cap.....Rs.450",fg="black",bg="skyblue").place(x=10,y=280)
    Label(f,font=("Arial",20,'bold'),text="Shoes.....Rs.1300",fg="black",bg="skyblue").place(x=10,y=320)

    #BILL
    f2=Frame(root,bg="light yellow",highlightbackground="black",highlightthickness=1,width=400,height=420) #frame for bill
    f2.place(x=950,y=345)

    Bill=Label(f2,text="Bill",font=("calibri",30,"bold"),bg="lightyellow")   
    Bill.place(x=165,y=5)

    #Entry
    f1=Frame(root,bd=5,height=500,width=300,relief=RAISED)  
    f1.place(x=510,y=345)

    Tshirt=StringVar()  #referenced as string variables
    Jeans=StringVar()    
    Shirt=StringVar()
    Jacket=StringVar()
    Mask=StringVar()
    Cap=StringVar()
    Shoes=StringVar()
    Total_bill=StringVar()
    Total_tax=StringVar()
    Total_cost=StringVar() 
    #Label
    lb0=Label(f1,font=("aria",20,"bold"),text="No. of items",width=12,fg="blue4")
    lb1_Tshirt=Label(f1,font=("aria",20,"bold"),text="T-shirt",width=12,fg="blue4")     
    lb2_Jeans=Label(f1,font=("aria",20,"bold"),text="Jeans",width=12,fg="blue4")
    lb3_Shirt=Label(f1,font=("aria",20,"bold"),text="Shirt",width=12,fg="blue4")
    lb4_Jacket=Label(f1,font=("aria",20,"bold"),text="Jacket",width=12,fg="blue4")
    lb5_Mask=Label(f1,font=("aria",20,"bold"),text="Mask",width=12,fg="blue4")
    lb6_Cap=Label(f1,font=("aria",20,"bold"),text="Cap",width=12,fg="blue4")
    lb7_Shoes=Label(f1,font=("aria",20,"bold"),text="Shoes",width=12,fg="blue4")

    lb0.grid(row=1,column=1)
    lb1_Tshirt.grid(row=2,column=0)                 #grids specify the position of the labels
    lb2_Jeans.grid(row=3,column=0)
    lb3_Shirt.grid(row=4,column=0)
    lb4_Jacket.grid(row=5,column=0)
    lb5_Mask.grid(row=6,column=0)
    lb6_Cap.grid(row=7,column=0)
    lb7_Shoes.grid(row=8,column=0)

    #Entry
    entry_Tshirt=Entry(f1,font=("aria",20,"bold"),textvariable=Tshirt,bd=6,width=8,bg="lightgreen")
    entry_Jeans=Entry(f1,font=("aria",20,"bold"),textvariable=Jeans,bd=6,width=8,bg="lightgreen")   #entries for the no. of items to buy
    entry_Shirt=Entry(f1,font=("aria",20,"bold"),textvariable=Shirt,bd=6,width=8,bg="lightgreen")
    entry_Jacket=Entry(f1,font=("aria",20,"bold"),textvariable=Jacket,bd=6,width=8,bg="lightgreen")
    entry_Mask=Entry(f1,font=("aria",20,"bold"),textvariable=Mask,bd=6,width=8,bg="lightgreen")
    entry_Cap=Entry(f1,font=("aria",20,"bold"),textvariable=Cap,bd=6,width=8,bg="lightgreen")
    entry_Shoes=Entry(f1,font=("aria",20,"bold"),textvariable=Shoes,bd=6,width=8,bg="lightgreen")

    entry_Tshirt.grid(row=2,column=1)
    entry_Jeans.grid(row=3,column=1)
    entry_Shirt.grid(row=4,column=1)
    entry_Jacket.grid(row=5,column=1)
    entry_Mask.grid(row=6,column=1)                   #positions
    entry_Cap.grid(row=7,column=1)
    entry_Shoes.grid(row=8,column=1)

    #BUTTONS for reset and total with their respective commands
    btn_reset=Button(f1,bd=5,fg="black",bg="lightblue",font=("ariel",16,"bold"),width=10,text="Reset",command=Reset)
    btn_reset.grid(row=9,column=0)

    btn_total=Button(f1,bd=5,fg="black",bg="lightblue",font=("airel",17,"bold"),width=10,text="Total",command=Total)
    btn_total.grid(row=9,column=1)


    root.mainloop()
    
#############################################################################################################################################   
#############################################################################################################################################   

#salary function for salary button
def salary():
    c1=Canvas(root,bg="skyblue",highlightbackground="black",highlightthickness=1,width=1900,height=1000,scrollregion=[0,0,10000,10000])

    Label(c1,text="Employees and their salaries",font=("Agency FB",45,"bold"),fg="black",bg="skyblue").place(x=80,y=5)

    vscrollbar=Scrollbar(root,orient="vertical")        #for vertical scrollbar
    c1.config(yscrollcommand=vscrollbar.set)
    vscrollbar.config(command=c1.yview)

    hscrollbar=Scrollbar(root,orient="horizontal")      #for horizontal scrollbar
    c1.config(xscrollcommand=hscrollbar.set)
    hscrollbar.config(command=c1.xview)

    hscrollbar.pack(side=BOTTOM,fill=X)
    vscrollbar.pack(side=RIGHT,fill=Y)                  #positions
    c1.place(x=10,y=230)
    
    #labels
    Label(c1,font=("Ariel",25,'bold'),text="Het-----2,50,000",fg="black",bg="skyblue").place(x=50,y=90)
    Label(c1,font=("Ariel",25,'bold'),text="Arya-----5,00,000",fg="black",bg="skyblue").place(x=50,y=150)
    Label(c1,font=("Ariel",25,'bold'),text="Charvi-----1,00,000",fg="black",bg="skyblue").place(x=50,y=210)
    Label(c1,font=("Ariel",25,'bold'),text="Sameer-----30,000",fg="black",bg="skyblue").place(x=50,y=270)
    Label(c1,font=("Ariel",25,'bold'),text="Kirtan------50,000",fg="black",bg="skyblue").place(x=50,y=330)
    Label(c1,font=("Ariel",25,'bold'),text="Maahika-----15,000",fg="black",bg="skyblue").place(x=50,y=390)
    Label(c1,font=("Ariel",25,'bold'),text="Ayush------20,000",fg="black",bg="skyblue").place(x=50,y=450)
#function for back button 
def back():
    f5=Frame(root,highlightthickness=1,width=1920,height=1080)
    f5.place(x=0,y=225)

#buttons with respective commands
btnBilling=Button(text='Billing',padx=2,pady=2,bd=2,fg="black",font=('arial', 10,'bold'), width=20, height=1,command=billing).pack()
btnsalary=Button(text='Salary',padx=2,pady=2,bd=2,fg="black",font=('arial', 10,'bold'), width=20, height=1,command=salary).pack()
btnBack=Button(text='Back',padx=2,pady=2,bd=2,fg="black",font=('arial', 10,'bold'), width=20, height=1,command=back).pack()
btnExit=Button(text='Exit',padx=2,pady=2,bd=2,fg="black",font=('arial', 10,'bold'), width=20, height=1,command=exit).pack()



