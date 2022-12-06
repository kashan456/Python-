# Python-
N=["HARSH","HEMASIS","KASHAN"]#list to store names of the student
M=[60,70,95]#list to store previous marks of the student

#finding previous rank of HARSH
if (M[0]>M[1] and M[0]>M[2]):
  pR_Harsh=1
elif (M[0]<M[1] and M[0]<M[2]):
  pR_Harsh=3
else:
  pr_Harsh=2
#finding previous rank of HEMASIS
if (M[1]>M[0] and M[1]>M[2]):
  pR_Hemasis=1
elif (M[1]<M[0] and M[1]<M[2]):
  pR_Hemasis=3
else:
  pR_Hemasis=2
#finding previous rank of KASHAN
if (M[2]>M[1] and M[2]>M[0]):
  pR_Kashan=1
elif (M[2]<M[1] and M[2]<M[0]):
  pR_Kashan=3
else:
  pr_Kashan=2  
print("Harsh previous rank:",pR_Harsh)
print("Kashan previous rank:",pR_Kashan)
print("Hemasis previous rank:",pR_Hemasis)
print("\n")
U=[80,75,60]#list to store updated marks of students
#rank of HARSH after updation
if (U[0]>U[1] and U[0]>U[2]):
  uR_Harsh=1
elif (U[0]<U[1] and U[0]<U[2]):
  uR_Harsh=3
else:
  uR_Harsh=2
#rank of HEMASIS after updation
if (U[1]>U[0] and U[1]>U[2]):
  uR_Hemasis=1
elif (U[1]<U[0] and U[1]<U[2]):
  uR_Hemasis=3
else:
  uR_Hemasis=2
#rank of KASHAN after updation
if (U[2]>U[1] and U[2]>U[0]):
  uR_Kashan=1
elif (U[2]<U[1] and U[2]<U[0]):
  uR_Kashan=3
else:
  uR_Kashan=2 
print("Harsh updated rank:",uR_Harsh)
print("Kashan updated rank:",uR_Kashan)
print("Hemasis updated rank:",uR_Hemasis)
print("\n")
if (U[0]>U[1] and U[0]>U[2]):
  print(N[0] +" ,JUMP:",pR_Harsh-uR_Harsh)
elif (U[1]>U[0] and U[1]>U[2]):
  print(N[1]+" ,Jump:",pR_Hemasis-uR_Hemasis)
elif (U[2]>U[0] and U[2]>U[1]):
  print(N[2]+" ,Jump:",pR_Kashan-uR_Kashan)
