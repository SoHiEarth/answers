# 解答

## 第2回
    def homework(w, d, h):
    
        return 1000 <= w*d*h

## 第3回
    def homework(a):
    
        return a[(a%5 == 0) & (a%2 == 1)]

## 第4回
    def homework(path, n):

        df = pd.read_csv(p, sep=';')

        df['tmp'] = pd.qcut(df["volatile acidity"], n)
    
        return df[df["quality"] == 5].groupby("temp")["alcohol"].mean().min()
