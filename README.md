# code
Python 3.11.7 (tags/v3.11.7:fa7a6f2, Dec  4 2023, 19:24:49) [MSC v.1937 64 bit (AMD64)] on win32
Type "help", "copyright", "credits" or "license" for more information.
>>> pip install flask
  File "<stdin>", line 1
    pip install flask
        ^^^^^^^
SyntaxError: invalid syntax
>>> pip install Flask
  File "<stdin>", line 1
    pip install Flask
        ^^^^^^^
SyntaxError: invalid syntax
>>> from tkinter import *
>>> from tkinter import messagebox
>>>
>>> root = Tk()
>>> root.minsize(width=1370, height=720)
>>> root.configure(background="dark gray")
>>>
>>> tops = Frame(root, width=1350, height=50, bd=8, bg="dark blue")
>>> tops.pack(side=TOP)
>>>
>>> f1 = Frame(root, width=600, height=600, bd=8, bg="dark gray")
>>> f1.pack(side=LEFT)
>>> f2 = Frame(root, width=300, height=700, bd=8, bg="dark blue")
>>> f2.pack(side=RIGHT)
>>>
>>> fla = Frame(f1, width=600, height=200, bd=8, bg="dark blue")
>>> fla.pack(side=TOP)
>>> flb = Frame(f1, width=300, height=600, bd=8, bg="dark blue")
>>> flb.pack(side=TOP)
>>>
>>> lbl_information = Label(tops, font=('arial', 45, 'bold'), text="Employee Payment Management System")
>>> lbl_information.grid(row=0, column=0)
>>>
>>>
>>> def Exit():
...     wayout = messagebox.askyesno("Employee Payment System", "Do you want to exit the system?")
...     if wayout > 0:
...         root.destroy()
...         return
...
>>> # You can add a button to trigger the Exit function
>>> exit_button = Button(root, text="Exit", command=Exit)
>>> exit_button.pack()
>>>
>>> root.mainloop()
>>>
