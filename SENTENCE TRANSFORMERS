from sentence_transformers import SentenceTransformer, util

# Load model
model = SentenceTransformer('all-MiniLM-L6-v2')

# Input texts
text1 = input("Enter Text 1: ")
text2 = input("Enter Text 2: ")

# Encode texts
embedding1 = model.encode(text1, convert_to_tensor=True)
embedding2 = model.encode(text2, convert_to_tensor=True)

# Cosine similarity
similarity = util.cos_sim(embedding1, embedding2)

score = float(similarity[0][0])

print("\nSimilarity Score:", round(score, 2))

# Similarity level
if score > 0.75:
    print("Similarity Level: High")
elif score > 0.40:
    print("Similarity Level: Medium")
else:
    print("Similarity Level: Low")
