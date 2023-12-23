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

# video

https://github.com/Yuvraj0444/videos-frames/assets/150776511/3de885ba-2377-4f05-a7b6-d77ebc0deaa8

