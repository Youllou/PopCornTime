#-------------------------------------------------------------------------------
# Name:        PopCornTime
# Purpose:
#
# Author:      Youllou, Oykard, Agathe
#
# Created:     26/03/2020
# Copyright:   (c) Youllou 2020
# Licence:     <your licence>
#-------------------------------------------------------------------------------

from tkinter import*


newMovie1='FilmA'
newMovie2='FilmB'
newMovie3='FilmC'
newMovie4='FilmD'
newMovie5='FilmE'
newMovie6='FilmF'



popCornTime=Tk()
popCornTime.title('PopCornTime')
popCornTime.geometry('1200x800')
popCornTime.configure(bg='white')




def menu():

    menu=Frame(popCornTime,bg="#00001a",width=1200,height=800)
    menu.pack()

    cadreTitrePage=Canvas(menu,bg="#ff9c59",width=540,height=100)
    cadreTitrePage.configure(highlightbackground="#ffbf95")
    cadreTitrePage.place(x=530,y=25)

    cadreRecherche=Canvas(menu,bg="#ff9c59",width=300,height=125)
    cadreRecherche.configure(highlightbackground="#ffbf95")
    cadreRecherche.place(x=1,y=300)

    recherche=Text(menu,width=32,height=2)
    recherche.insert(END,"Rechercher")
    recherche.config(font='arial 12')
    recherche.place(x=2,y=345)

    cadreMesFilms=Button(menu,bg="#ff9c59",width=42,height=8)
    cadreMesFilms.configure(highlightbackground="#ffbf95")
    cadreMesFilms.place(x=1,y=525)

    nouveau=Canvas(menu,bg="#00001a",width=540,height=470)
    nouveau.configure(highlightbackground='#ffbf95')
    #on creer le canevas comportant les nouveaux films
    nouveau.place(x=530,y=280)

    quitter=Button(menu,width=5,height=1,text='Quitter')
    quitter.configure(command=popCornTime.destroy)
    quitter.place(x=1100,y=750)

    photo=PhotoImage(file="Logo Pop Corn Time.png")
    logo=Label(menu,width=175,height=150,image=photo,bg="#00001a",activebackground="#00001a")
    logo.configure(border=0)
    logo.place(x=2,y=1)

    def Onglet(coordx,coordy,movieName):
        """fonction créant des onglets de même taille et de même couleur puis les places à des coordonnées définies
        on réduit ainsi la taille du programme en répétant une tache
        """
        onglet=Button(menu,bg="#00001a",width=20,height=13,command=lambda:ficheFilm(nomDuFilm))
        onglet.configure(highlightbackground="#ff9b59")
            #la commande "command=lambda:..." permet l'affichage de la seconde fenêtre avec l'info du nom du film
            #le "lambda" permet l'ajout d'une variable à la fonction
        onglet.place(x=coordx,y=coordy)


    film1=Onglet(550,300,newMovie1)
    film2=Onglet(725,300,newMovie2)
    film3=Onglet(900,300,newMovie3)
    film4=Onglet(550,525,newMovie4)
    film5=Onglet(725,525,newMovie5)
    film6=Onglet(900,525,newMovie6)
        #ici, pour chaque film, on appel la fonction en donnant la position en x, en y et le nom du film


menu()
popCornTime.mainloop()
