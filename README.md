start = Time.now
def radixSort(array)
	temp = Array.new

	array.each do |x|
		if temp[x] == nil
			temp[x] = 1
		else
			temp[x] = temp[x] + 1
		end
	end

	temp.each_with_index do |x, i|
		if (x)
			x.times do
				puts i
			end
		end
	end
end

def run()
	test = [25,24,23.22,21,20,19,18,17,16,15,14,13,12,11,10,9,8,7,6,5,4,3,2,1]
	radixSort(test)
end

run
finish = Time.now
diff = finish - start
#puts diff
gets
