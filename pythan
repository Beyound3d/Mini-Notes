from tkinter import *

root = Tk()
root.title("Notes App")

# Create a text box for the user to input notes
note_box = Text(root, height=20, width=50)
note_box.pack()

# Create a button to save the notes
def save_notes():
    notes = note_box.get("1.0", END)
    with open("notes.txt", "w") as f:
        f.write(notes)

save_button = Button(root, text="Save Notes", command=save_notes)
save_button.pack()

root.mainloop()
