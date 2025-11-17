import tkinter as tk
from html.entities import entitydefs
from tkinter import ttk
from tkinter import messagebox

window = tk.Tk()
window.geometry("500x450")
window.title("Welcome to First App")

def buttonFunction():
     print("push button")
     label.config(text = "hello",
                  fg = "green",
                  bg = "blue",
                  font = "times 30"
                  )
     value = entry.get()
     print(value)
     label.configure(text = value)
     #message_box = messagebox.showinfo(title= "info", message="sıkıntı var")
     message_box = messagebox.askyesnocancel(title="info", message= "information")
     print(message_box)



#BUTTON

button = tk.Button(window, text = "Welcome guys", activebackground="red",
                   bg= "black", fg = "white", activeforeground= "black",
                   height= 15 , width = 50,
                   command= buttonFunction)
button.pack()

#LABEL
label = tk.Label(window, text = "HI WORLD" , font = "times 18",
                 fg= "red",bg= "black",
                 wraplength=200)

label.pack(side = tk.RIGHT, padx= 35)

# ENTRY

entry = tk.Entry(window, width=70)
entry.insert(string = "write something only one time", index = 0)
entry.pack(side = tk.LEFT, padx= 20)
















window.mainloop()
