# Interests
> This will mostly about me talking about my interests
## Books
> I really love to read books, mostly about fictional stories and adventures. Never really was interested in the romance novels to be honest. I have read many books over the years but there are some that stuck with me more then others.
> Here are some of the authors that created some of my favorite books:
* Rick Riordan
* J.K Rowling
* Kelly Armstrong
* ETC....

## Specific Books
> The Specific books that I like to read from these authors are:
* [The Summoning Series](https://www.kelleyarmstrong.com/book/the-summoning/)
* [The Kane Chronicles](https://rickriordan.com/series/kane-chronicles/)
* [The Heroes of Olympus](https://en.wikipedia.org/wiki/The_Heroes_of_Olympus)
* [Harry Potter](https://en.wikipedia.org/wiki/Harry_Potter)
> There are some other books that I have read that also interested me, but these books are what I perceive as my favorites during my time reading them.

## Video Games
> I love to play video games as well especially roleplaying games or games of survival as well.
> Normally I would actually play these games on my tablet and not on my computer or phone because, the computer only has limited storage and the phone may end up lose memory storage as well. 
> the tablet may need storage as well but its not used for important stuff as the phone and computer so it doesn't really matter what games it has.
### These Games are:
* [Fortnite](https://cdn1.epicgames.com/salesEvent/salesEvent/18BR_S18_Launcher_EGS_Blade_2560x1440_2560x1440-da6f6a137b90887357222b762c7675a1?h=270&resize=1&w=480)
* [Genshin Impact](https://cdn1.epicgames.com/salesEvent/salesEvent/EGS_GenshinImpact_miHoYoLimited_S1_2560x1440-91c6cd7312cc2647c3ebccca10f30399)
* [PubG](https://play-lh.googleusercontent.com/JRd05pyBH41qjgsJuWduRJpDeZG0Hnb0yjf2nWqO7VaGKL10-G5UIygxED-WNOc3pg)
* ![Monster Legends](https://play-lh.googleusercontent.com/e5YrwWQOcF-TGUF7rLKGoq4cd4o94W4JBPXrRTsvgnVCCl8RhAH8YDMZwDDkzbDgxBk)
* ![Dragon City](https://static.tvtropes.org/pmwiki/pub/images/dragon_city_logo.png)

# Explanation
> The 2 images are the logos of my favorite games the other 3 are linked to the logos of those games as well to show what they look like and see if you are interested in playing those games. Fortnite can not be played on IOS due to a problem with the company Apple against the creators company Epic Games. The rest of the games can be played on both platforms of IOS and Android. Fortnite, PubG and Genshin Impact can also be played on laptops or computers if you want to play on them there.

# Coding
> This is what actually got me into coding because I actually always wanted to know how certain elements of the game work behind the scenes of the 3D or 2D characters.
> Like this code here, it allows to insert any amount of numbers and automatically creates a new file:
import random

def generateRandomNumber(min_num,max_num):
    
    randomNumber = random.randint(min_num,max_num)
    return randomNumber
def main():
    
    while True:
        try:
            numberOfRandomNumbers = int(input("How many numbers" + \
                                      " should the file hold?: "))
            min_num = float(input("What is the Minimum number? "))
            max_num = float(input("What is the Maximum number? "))
            fileToBeWritten = open("randomNumbers.txt","w")
            if (numberOfRandomNumbers < 0):
                print("Positive integers only")
                break 
        except Exception as error:
            print("There was an error", error)
        else:
            for randomNumberCount in range(1, numberOfRandomNumbers + 1):
                randomNumber = generateRandomNumber(min_num,max_num) 
                fileToBeWritten.write(str(randomNumber)+ "\n")
                

        print(numberOfRandomNumbers,  "numbers have been written in the file.")
        break
main()
