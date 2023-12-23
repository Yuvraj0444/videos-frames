# videos-frames
import cv2

cap=cv2.VideoCapture("C:/Users/asus/Desktop/Venice_10.mp4") #location of video

i=0
while(cap.isOpened()):
    flag,frame=cap.read()
    if flag==False:
        break
    path='D:/frames/number of frames'+str(i)+'.jpg' #location of the folder where the frames will be saved
    cv2.imwrite(path,frame)
    i+=1

cap.release()
cv2.destroyAllWindows()


