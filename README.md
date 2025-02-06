# ANNlab
def artificial_neuron(inputs, weights, bias):
    weighted_sum = 0
    
    for i in range(len(inputs)):
        weighted_sum += inputs[i] * weights[i]
    weighted_sum += bias
       
    output = 1 if weighted_sum > 0 else 0

    return output

# Inputs for AND operator
inputs = [1, 1]
weights = [1, 1]
bias = -1.5

output = artificial_neuron(inputs, weights, bias)
print("Neuron output:", output)
