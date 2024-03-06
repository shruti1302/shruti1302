# Define sample medical data for disease prediction
patient_data = {
    'age': 45,
    'gender': 'Male',
    'blood_pressure': 'High',
    'cholesterol': 'High',
    'symptoms': ['Chest pain', 'Shortness of breath'],
    'family_history': True
}

# Define rules for disease prediction based on the medical data
def predict_disease(patient_data):
    if patient_data['age'] > 40 and patient_data['gender'] == 'Male' and patient_data['blood_pressure'] == 'High' and patient_data['cholesterol'] == 'High' and 'Chest pain' in patient_data['symptoms'] and patient_data['family_history']:
        return "Heart Disease"
    else:
        return "No specific disease predicted"

# Predict the disease based on the sample medical data
predicted_disease = predict_disease(patient_data)
print("Predicted Disease:", predicted_disease)
