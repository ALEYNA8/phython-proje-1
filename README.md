# phython-proje-1
1.GÖREV: BİR LİSTEYİ DÜZLEŞTİREN (FLATTEN) FONKSİYON YAZMA:
def flatten(lst):
    result = []
    for item in lst:
        if isinstance(item, list):
            result.extence(flatten(item)) 
        else:
            result.append(item)
    return result
    # TEST
    input_list = [[1, 'a', ['cat'],2], [[3]], 'dog'], 4, 5]
    output = flatten(input_list)
    print(output)

    2. GÖREV: VERİLEN LİSTEYİ VE İÇİNDEKİ LİSTELERİ TERSİNE ÇEVİRME:
    def reverse_nested_list(lst):
        result = []
        for item in lst[::-1]:
            if isinstance(item, list):
               result.append(reverse_nested_list(item))
            else:
                 result.append(item)
            return result
            # TEST
            input_list = [[1,2], [3,4], [5,6,7]]
            output = reverse_nested_list(input_list)
            print(output)



            ÇIKTILAR:
            1.GÖREV;
            [1, 'a', 'cat', 2, 3, 'dog',4, 5]

            2.GÖREV;
            [[[7, 6, 5], [4, 3], [2, 1]]]
            
    
