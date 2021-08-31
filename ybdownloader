from tkinter import *
from pytube import YouTube
def download():   
    url =YouTube(str(link_enter.get()))
    video = url.streams.first()
    video.download()
    Label(window, text = 'DOWNLOADED', font = 'arial 15').place(x= 210, y = 250) 

window = Tk()
window.geometry("600x300")
window.resizable(0,0)
window.title("Youtube downloader")
Label(window,text="Youtube Downloader",font=("Arial",25)).pack()
text = StringVar()
label1 = Label(window,text="Enter Your link",font=("Arial",25))
label1.place(x= 190, y = 60)
link_enter = Entry(window,width=70,textvariable=text)
link_enter.place(x=80, y=160)
button = Button(window,text="Download",font=("Arial",15),command=download)
button.place(x=240, y=200)



window.mainloop()
