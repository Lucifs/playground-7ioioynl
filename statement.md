from time import *
def random(m):
    s= perf_counter()
    n = perf_counter() * 20154864857
    return int(n)%m
def creerGrille(nombreLignes, nombreColonnes):
    grid = [[]] * nombreLignes
    for ligne in range(nombreLignes):
        grid[ligne] = [0] * nombreColonnes
    return grid
def affichage(g):
    for i in g:
        print(i)
def alpha(g):
    c=0
    for i in range(len(g)):
        for j in range(len(g[i])):
            g[i][j] = chr(97+c)
            c+=1
def creerGrilleNombresAleatoires(g):
    for i in range(len(g)):
        for j in range(len(g[i])):
            g[i][j] = random(10)
