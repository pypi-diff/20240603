# Comparing `tmp/matplobblib-0.1.3.tar.gz` & `tmp/matplobblib-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplobblib-0.1.3.tar", last modified: Tue May 28 11:42:50 2024, max compression
+gzip compressed data, was "matplobblib-0.1.4.tar", last modified: Mon Jun  3 08:45:59 2024, max compression
```

## Comparing `matplobblib-0.1.3.tar` & `matplobblib-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 11:42:50.984483 matplobblib-0.1.3/
--rw-rw-rw-   0        0        0       38 2024-05-26 12:40:51.000000 matplobblib-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0       18 2024-05-26 10:39:36.000000 matplobblib-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      406 2024-05-28 11:42:50.984483 matplobblib-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       37 2024-05-28 09:22:25.000000 matplobblib-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 11:42:50.976757 matplobblib-0.1.3/matplobblib/
--rw-rw-rw-   0        0        0       35 2024-05-28 11:41:45.000000 matplobblib-0.1.3/matplobblib/__init__.py
--rw-rw-rw-   0        0        0    27912 2024-05-28 11:40:59.000000 matplobblib-0.1.3/matplobblib/package.py
-drwxrwxrwx   0        0        0        0 2024-05-28 11:42:50.982594 matplobblib-0.1.3/matplobblib.egg-info/
--rw-rw-rw-   0        0        0      406 2024-05-28 11:42:50.000000 matplobblib-0.1.3/matplobblib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2024-05-28 11:42:50.000000 matplobblib-0.1.3/matplobblib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 11:42:50.000000 matplobblib-0.1.3/matplobblib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-28 11:42:50.000000 matplobblib-0.1.3/matplobblib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-05-28 11:42:50.985483 matplobblib-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      596 2024-05-28 11:42:33.000000 matplobblib-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:45:59.905604 matplobblib-0.1.4/
+-rw-rw-rw-   0        0        0       38 2024-05-26 12:40:51.000000 matplobblib-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       18 2024-05-26 10:39:36.000000 matplobblib-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      406 2024-06-03 08:45:59.905604 matplobblib-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2024-05-28 09:22:25.000000 matplobblib-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 08:45:59.899713 matplobblib-0.1.4/matplobblib/
+-rw-rw-rw-   0        0        0       35 2024-05-28 11:41:45.000000 matplobblib-0.1.4/matplobblib/__init__.py
+-rw-rw-rw-   0        0        0    28303 2024-06-03 08:43:49.000000 matplobblib-0.1.4/matplobblib/package.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:45:59.905604 matplobblib-0.1.4/matplobblib.egg-info/
+-rw-rw-rw-   0        0        0      406 2024-06-03 08:45:59.000000 matplobblib-0.1.4/matplobblib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2024-06-03 08:45:59.000000 matplobblib-0.1.4/matplobblib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 08:45:59.000000 matplobblib-0.1.4/matplobblib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-06-03 08:45:59.000000 matplobblib-0.1.4/matplobblib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-06-03 08:45:59.907110 matplobblib-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      596 2024-06-03 08:45:37.000000 matplobblib-0.1.4/setup.py
```

### Comparing `matplobblib-0.1.3/matplobblib/package.py` & `matplobblib-0.1.4/matplobblib/package.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import pyperclip
-
-#Делаем функцию которая принимает переменную text
-def write(name):
-    pyperclip.copy(name) #Копирует в буфер обмена информацию
-    pyperclip.paste()
-
 def description():
     themes = {'Непрерывные случайные величины': ['CRV_1()', 'CRV_2()'],
               'Нормальные случайные векторы': ['NRV_1()', 'NRV_2()', 'NRV_3()'],
               'Формулы полной вероятности и Байеса':['FPB_1()','FPB_2()','FPB_3()','FPB_4()'],
               'Специальные дискретные случайные величины':['SDRV_1()','SDRV_2()','SDRV_3()','SDRV_4()'],
               'Условные характеристики относительно группы событий':['CCE_1()','CCE_2()'],
-              'Приближенное вычисление вероятности методом Монте-Карло':['ACMK_1()','ACMK_2()','ACMK_3()','ACMK_4()']
+              'Приближенное вычисление вероятности методом Монте-Карло':['ACMK_1()','ACMK_2()','ACMK_3()','ACMK_4()'],
+              'Включить функцию для добавления в буфер обмена': 'enable_ppc'
               }
     text = ""
     for key in themes.keys():
         text += f'{key}: '
         for f in themes[key]:
             text += f'{f}; '
         text += '\n'
     print(text)
-    
+def enable_ppc():
+    return '''    import pyperclip
+
+    #Делаем функцию которая принимает переменную text
+    def write(name):
+        pyperclip.copy(name) #Копирует в буфер обмена информацию
+        pyperclip.paste()'''    
 #ContinuousRandomVariables
 def CRV_1():
     task = 'Абсолютно непрерывная случайная величина  X  может принимать значения только в отрезке [a, b]. На этом отрезке плотность распределения случайной величины  X  имеет вид: f(x)=C(1+a^0.1+2b^0.2+3c^0.3)^1.1, где С - положительная константа. Найти:\n- константу C математическое ожидание E(X)\n- стандартное отклонение σX\n- квантиль уровня k распределения X'
     answer = '\n#условие\n# [a,b]\na,b = 4,9\n# F = f(x) без C\nF = lambda x: (1 + 7*x**(0.5) + 8*x**(0.7) + 4*x**(0.9))**(1.3)\nC = 1 / integrate.quad(F, a, b)[0]\ndef f(x):\n    return C * F(x)\nclass dist_f_C(rv_continuous):\n  #функция вероятности\n  def _pdf(self,x):\n    return f(x) if (a<= x <=b) else 0\n  #функция значений\n  def _expect(self,x):\n    return x\n#зададим распределение\nf_C = dist_f_C(a = a, b = b)\n#1\nprint(f"C = {C}")\n#2\nprint(f"E = {f_C.mean()}")\n#3\nprint(f"sigma = {f_C.std()}")\n#4\nprint(f"q = {f_C.ppf(0.9)}")\n'
     return [task,answer]
 def CRV_2():
     task = 'Случайная величина X равномерно распределена на отрезке [a,b]. Случайная величина Y выражается через X следующим образом: Y = (1+a^0.1+2b^0.2+3c^0.3)^1.1. Найдите:\n- математическое ожидание  E(Y)\n- стандартное отклонение σY\n- асимметрию As(Y)\n- квантиль уровня 0,8 распределения Y'
@@ -38,15 +38,39 @@
     return [task,answer]
 def NRV_2():
     task = 'Для нормального случайного вектора (X,Y)∼N(−4;4;64;81;−0,31) найдите вероятность P((X−8)(X−10)(Y−1)<0).'
     answer = "\n#Смотрим на распределение, которое задано\nmuX = -4\nmuY = 4\nsigmaX = 64**0.5\nsigmaY = 81**0.5\nrho = -0.31\n#Смотрим на вероятность, которую хотят от нас\nxminus1 = 8\nxminus2 = 10\nyminus = 1\nmu = np.array([muX,muY])\nCov = np.array([[sigmaX**2, rho*sigmaX*sigmaY], [rho*sigmaX*sigmaY, sigmaY**2]])\nX = norm(muX, sigmaX)\nY = norm(muY, sigmaY)\nW = multivariate_normal(mu, Cov)\nPa = W.cdf([xminus1, yminus])\nPb = X.cdf(xminus2) - X.cdf(xminus1) - (W.cdf([xminus2, yminus]) - W.cdf([xminus1, yminus]))\nPc = Y.cdf(yminus) - W.cdf([xminus2, yminus])\nPa+Pb+Pc\n"
     return [task,answer]
 def NRV_3():
     task = 'Случайный вектор (X,Y) имеет плотность распределения fX,Y(x,y)=(18e^(−30x2−48xy+8x−30y2−5y−8524))\π\nНайдите:\n- математическое ожидание E(X)\n-математическое ожидание E(Y)\n-дисперсию  Var(X)\n-дисперсию  Var(Y)\n-ковариацию  Cov(X,Y)\n-коэффициент корреляции  ρ(X,Y)'
-    answer = "\n#после выноса -1/2!!!!!!\ncoefs = {\n    'x^2': 60,\n    'x': -16,\n    'xy': 96,\n    'y': 10,\n    'y^2': 60,\n}\nC = np.matrix([[coefs['x^2'], coefs['xy']/2], [coefs['xy']/2, coefs['y^2']]])\nC1 = C**(-1)\nVarX = C1[0, 0]\nsigmaX = np.sqrt(VarX)\nVarY = C1[1, 1]\nsigmaY = np.sqrt(VarY)\nCovXY = C1[0, 1]\nroXY = CovXY/(sigmaX*sigmaY)\nEX, EY = sympy.symbols('EX, EY')\nequations = (\n    sympy.Eq(coefs['x^2']*EX + coefs['xy']/2*EY, coefs['x']*(-1/2)),\n    sympy.Eq(coefs['xy']/2*EX + coefs['y^2']*EY, coefs['y']*(-1/2))\n)\nsol = sympy.solve(equations, (EX, EY))\nprint(f'EX = {sol[EX]}, EY = {sol[EY]}, VarX = {VarX}, VarY = {VarY}, CovXY = {CovXY}, roXY = {roXY}')\n"
+    answer = '''
+            #после выноса -1/2!!!!!!
+        coefs = {
+            'x^2': 60,
+            'x': -16,
+            'xy': 96,
+            'y': 10,
+            'y^2': 60,
+        }
+        C = sympy.Matrix([[coefs['x^2'], int(coefs['xy']/2)], [int(coefs['xy']/2), coefs['y^2']]])
+        C1 = C**(-1)
+        VarX = C1[0, 0]
+        sigmaX = sympy.sqrt(VarX)
+        VarY = C1[1, 1]
+        sigmaY = sympy.sqrt(VarY)
+        CovXY = C1[0, 1]
+        roXY = CovXY/(sigmaX*sigmaY)
+        EX, EY = sympy.symbols('EX, EY')
+        equations = (
+            sympy.Eq(int(coefs['x^2'])*EX + int(coefs['xy']/2)*EY, int(coefs['x']*(-1/2))),
+            sympy.Eq(int(coefs['xy']/2)*EX + int(coefs['y^2'])*EY, int(coefs['y']*(-1/2)))
+        )
+        sol = sympy.solve(equations, (EX, EY))
+        print(f'EX = {sol[EX]}, EY = {sol[EY]}, VarX = {VarX}, VarY = {VarY}, CovXY = {CovXY}, roXY = {roXY}')
+        '''
     return [task,answer]
 
 #FullProbabilityAndBayesianFormulas
 def FPB_1():
     task = 'Имеется 37 монет, из которых 6 бракованные: вследствие заводского брака на этих монетах с обеих сторон отчеканен герб. Наугад выбранную монету, не разглядывая, бросают несколько раз. 1) Какова вероятность, что при 4 бросках она ляжет гербом вверх? 2) При 4 бросках монета легла гербом вверх. Какова вероятность того, что была выбрана монета с двумя гербами?'
     answer ='''
     coins = [('O', 'P')]*31 + [('O', 'O')]*6
@@ -216,15 +240,15 @@
     sigmaY=0.9
     sigmaZ=1.8
 
     AX = sigmaX**2
     AY = sigmaY**2
     AZ = sigmaZ**2
 
-    S = sts.poisson(AX + AY + AZ)
+    S =  poisson(AX + AY + AZ)
     #1
     print(rrstr(S.pmf(7),3),'P(S=7) ')
     #2
     print(S.median(),'Наиболее вероятное S ')
     #3
     print(rrstr(S.std(),3),'стандартное отклонение σS ')
     #4
@@ -266,15 +290,15 @@
         return mt.comb(n,k)
 
     #Дано
     N = 11
     n = 14
     G = 5
 
-    M = sts.geom(1/2 ** N * C(N,G))
+    M = geom(1/2 ** N * C(N,G))
 
     #1
     print(rrstr(M.mean(),3),'Математическое ожидание X')
     #2
     print(rrstr((M.var())**0.5,3),'Стандартное отклонение X')
     #3
     print(rrstr(M.var()/(M.std() * (n*M.var())**0.5),3),'Коэффициент корреляции X и Y')
@@ -301,29 +325,29 @@
     n = 12
 
     Ex = X/N * n
     Ey = Y/N * n
     Z = N - X - Y
 
     def C(n,k):
-    return mt.comb(n,k)
+        return math.comb(n,k)
 
 
     dXY = dict()
     for i in range(X+1):
         for j in range(Y+1):
             for k in range(Z+1):
                 if (i+j+k)==n:
                     p = C(X,i)*C(Y,j)*C(Z,k)/C(N,n)
                     dXY.setdefault(i*j,0)
                     dXY[i*j]+=p
 
     val = [i for i in dXY.keys()]
     chn = [i for i in dXY.values()]
-    Exy = sts.rv_discrete(values=(val,chn)).mean()
+    Exy = rv_discrete(values=(val,chn)).mean()
     print(rrstr(Exy - Ex*Ey,2))
     '''
     return [task,answer]
 
 #ConditionalCharacteristicsOfEvents
 def CCE_1():
     task='''
```

### Comparing `matplobblib-0.1.3/setup.py` & `matplobblib-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   with open('README.md', 'r') as f:
     return f.read()
 
 
 
 setup(
     name='matplobblib',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     description='A very simple TVIMS library',
     author='Ackrome',
     author_email='ivansergeyevicht@gmail.com',
     url='https://github.com/Ackrome/matplobblib',
     classifiers=[
         'Programming Language :: Python :: 3',
```

