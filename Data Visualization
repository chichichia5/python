import pandas as pd
from matplotlib import pyplot as plt

def main():
    df= pd.read_csv("./data/data.csv")
    print(df)
    hate= df["again"] == 2
    result = df['nation'][hate].value_counts()
    result = result.rename({1:"JP",2:"CH",3:"KR",50:"SG",51:"ML",52:"IND",53:"PH",54:"THAI",55:"VN",59:"INDIA",60:"USA",71:"GER, ENG, FRE",72:"EU",80:"AUS",88:"ROC",90:"Others"})
    plt.bar(result.index,result.values)
    #plt.xticks(rotation=60)
    plt.title("Nationalities of Those Who Don't Want to Visit Taiwan Again.")
    plt.xlabel('Nationality')
    plt.ylabel('Numbers')
    plt.savefig('Nationality.png')



if __name__ == "__main__":
    main()
