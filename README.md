

# 🔥 Steganography


![Header](https://user-images.githubusercontent.com/55437834/115628460-7ad61c80-a322-11eb-8095-a2bf03171db8.jpg)


Steganography is  process that is use for hiding  information inside of Image, audio , video or any digital object.That means  when you hide your informaton inside image or audio or video   , then send it to your destination  it's called steganograpghy   .

#### 👀 See detials Via Video : https://youtu.be/Kxwzy2bJCqk
 
### ▶️ Tools :
    
    steghide
    stegoveritas
    zsteg
    binwalk
    exiftool
    strings command
    stegsolver
    diit-1.5.jar
    formost
    sonic visualizer
    magic eye solver
    
    
### 🥇 Steghide :

Steghide is one of the most famous steganography tools, and for good reason. It's a classic method, hiding a message inside an image, and steghide does it effectively and efficiently. A downside of steghide is that it only works on jpgs; however, that means that if you believe there is a hidden message inside a jpg, then steghide is a probable option.



One of the greatest benefits of stegohide, is that it can encrypt data with a passphrase. Meaning that if they don't have the password then they can't extract any data.



#### Note :steghide can be installed with the command 👁️
                                                         sudo apt install steghide
     
##### Conclusion :
    
    steghide mainly use for extract or embeded file into .jpg file . But one can extract information from  audio / wav /mp3 file .
    So we can said that "Steghide  is  a  steganography  program  that  is able to hide data in various kinds of image- and audio-files"
    To embed emb.txt in cvr.jpg:
                                steghide embed -cf cvr.jpg -ef emb.txt
    To extract embedded data from stg.jpg:
                                          steghide extract -sf stg.jpg
     
    See details using man command (man steghide )
             
            
         
#### Note : Steghide can't extract .png format hide data 



              
### 🥈 Zsteg :
zsteg is to png's what steghide is to jpg's. It supports various techniques to extract any and all data from png files.



### Note: zsteg also supports BMP files, but it is primarily used for png's.



##### zsteg can be installed by using ruby with the command:
                                                           gem install zsteg
       
### Command : 
         
              zsteg image.png

### 🥉 Stegoveritas :
Personally this is one of my favorite image stego tools. It supports just about every image file, and is able to extract all types of data from it. It is an incredibly useful tool if you don't know exactly what you're looking for, as it has a myriad of built in tests to extract any and all data.



### Note: Stegoveritas has other features as well such as color correcting images



##### Stegoveritas can be installed by running these two commands:

                                                            sudo pip3 install stegoveritas 

                                                            stegoveritas_install_deps                
                  

              
### ⏲️ Stegsolver :
stegsolver is another important tools for Steganography CTF Challenges  . It change color combination and expose data from image .

#### 👁️‍🗨️ Download Link : https://github.com/zardus/ctf-tools/blob/master/stegsolve/install
             
#### Command :
              java -jar  stegsolver
             
Then , Choose target image and change color combination . If color changes system don't expose data you must click on  analyse button then choose option one by one . 

#### Note : You can combine two magic image for getting information using stegsolver

### 😆 Binwalk :
Binwalk use for different purpose  .In steganography we will use Binwalk for extract information without password . That means , when we have no password for extract image  , we will use " Binwalk " for extracting information . ( It's default on Kali Linux )

#### Command :
              binwalk -e image.jpg
         
#### 😍 See details via youtube video :https://youtu.be/ANMp1EHuXCY

### 🔥 Diit-1.5.jar :
diit-1.5.jar is so important tools for CTF contest . When all process fail to solve steganograhy challenge it come .
It use algorithm for extract data from image file

##### 💩 Download Link :http://diit.sourceforge.net/
     
#### Command :
              java -jar diit-1.5.jar

### 🧑‍🚀 Magic eye solver:
     magic eye solver is onle tools which is similar tools like stegsolver .It is mainly use for magic image .
                 
#### 👓 Website Link :https://magiceye.ecksdee.co.uk/


#### How to solve Challenge of Steganography ?

Ok  , no problem . Follow the given below process >>

### 👀 Process for solving Steganography image  Challenges :

Step 1: check file type using  file command

Step2:use exiftool command 

Step3:use strings command

Step4:use steghide command if you have password for extract  otherwise use binwalk (But luckly you can try steghide without password)

Step5:zsteg tools 

Step6:open stegsolve.jar file using java –jar stegsolve.jar ( then  , try to use it according to its uses )

Step7:use magic eye solver 

Step8:use diit-1.5.jar and try to extract information 

### 😍 Process for solving Steganography wav  Challenges :

Step 1 :open  file and listen it .

Step 2 :If target audio file is morse code try to extract information using online morse code decode tools .If not , follow step 3

Step 3 :open sonic visualizer and try to extract information from it .

Step 4 : If above all step are failed . Try to extract data using  steghide as it has ability to extract audio file 


## 👁️‍🗨️Bonus :
#### Stegcracker :
Stegcracker use for crack password of image.jpg format file . That means  when  we have no password and we can't extract information using Binwalk tools  we will use stegcracker for crack password of target file . It is so important tools in stego .


😍 Happy Hacking 👀
