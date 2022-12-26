# submit-delete-backspace
how to write on a screen, delete and backspace


from tkinter import *

window= Tk()

def submit():
    catch= entry.get()
    print(catch)
def delete():
    entry.delete(0,END)
def backspace():
    entry.delete(len(entry.get())-1,END)


entry= Entry(window,font="Arial,30")
entry.pack(side=LEFT)
submit_button = Button(window,font='Arial,20',command=submit,bg='black',
                                           text='submit',fg='blue')
submit_button.pack(side=RIGHT)
delete_button = Button(window,font='Arial,20',command=delete,bg='black',
                                           text='delete',fg='blue')
delete_button.pack(side=RIGHT)
Backspace = Button(window,font='Arial,20',command=backspace,bg='black',
                                           text='backspace',fg='blue')
Backspace.pack(side=RIGHT)

window.mainloop()
