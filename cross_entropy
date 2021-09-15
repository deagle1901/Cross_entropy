from math import log
def cross_entropy(actual, predicted):
    sum_score = 0.0
    for i in range(len(actual)):
        for j in range(len(actual[i])):
            sum_score += actual[i][j] * log(1e-15 + predicted[i][j])
    mean_sum_score = 1.0/len(actual) * sum_score
    return -mean_sum_score
actual = [[0],[0],[0],[1],[1],[1],[0],[1],[1],[0]]
predicted = [[0.77330069, 0.41045362, 0.11336399],
 [0.33767255, 0.84421107, 0.41008781],
 [0.96718145, 0.0899926,  0.07174224],
 [0.02052135, 0.77886221, 0.70268842],
 [0.64919759, 0.30145436, 0.04102113],
 [0.68973698, 0.58821819, 0.10546255],
 [0.29698513, 0.43547422, 0.28529975],
 [0.2968849,  0.61283841, 0.63136324],
 [0.32357182, 0.13638021, 0.90788238],
 [0.89679202, 0.97985175, 0.11401821]]

print(cross_entropy(actual, predicted))
