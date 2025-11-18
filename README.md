import tkinter as tk

win = tk.Tk()
win.geometry("300x300")
win.title("Canlarım")

label1 = tk.Label(win, text="rzg", bg ="red")
label2 = tk.Label(win,text = "ccn", bg ="light pink")
label3 = tk.Label(win,text = "Rüzgar", bg ="blue")

label1.place(x = 30, y = 30, width = 120, height = 70)
label2.place(x = 100, y = 100, width = 70, height = 70)
label3.place(x = 180, y = 180, width = 180, height = 170)




win.mainloop()

