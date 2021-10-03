# Dsa-3-

#include<stdio.h>

void main()
{ 
 int A[2][2],B[2][2],add[2][2],sub[2][2],product[2][2],trans[2][2], i,
    j,k,sum=0;
  printf("enter the first matrix");
  for(i=0;i<2;i++)
    for(j=0;j<2;j++)
      scanf ("%d",&A[i][j]);
  printf("enter the second matrix");
  for(i=0;i<2;i++)
    for(j=0;j<2;j++)
      scanf("%d",&B[i][j]);

  printf("the first matrix is\n");
  for(i=0;i<2;i++)
  {
    for(j=0;j<2;j++)
	{
	  printf("\t%d",A[i][j]);
	}
      printf("\n");
  }

  printf("the second matrix is\n");
  for(i=0;i<2;i++)
  {
    for(j=0;j<2;j++)
	{
	  printf("\t%d",B[i][j]);
	}
      printf("\n");
  }
  printf("sum of matrix is\n");
  for(i=0;i<2;i++)
  {
    for(j=0;j<2;j++)
	{
	  add[i][j]=A[i][j]+B[i][j];
	  printf("\t%d",add[i][j]);
	}
      printf("\n");
  }
  printf("subtraction of matrix is\n");
  for(i=0;i<2;i++)
  {
    for(j=0;j<2;j++)
	{
	  sub[i][j]=A[i][j]-B[i][j];
	  printf("\t%d",sub[i][j]);
	}
      printf("\n");
  }
  printf("product of matrix is\n");
  for(i=0;i<2;i++)
  {
    for(j=0;j<2;j++)
	{
	  sum=0;
	  for(k=0; k<2;k++)
	    sum=sum+A[i][k]*B[k][j];
	  product[i][j] = sum;
	}
  }
  for(i=0;i<2;i++)
  {
    for(j=0;j<2;j++)
	{
	  printf("\t%d",product[i][j]);
	}
      printf("\n");
  }
  printf("transpose of first matrix is\n");
  for(i=0;i<2;i++)
  {
    for(j=0;j<2;j++)
	{
	  trans[i][j]=A[j][i];
	  printf("\t%d",trans[i][j]);
	}
      printf("\n");
  }
  printf("transpose of second matrix is\n");
  for (i=0;i<2;i++)
  {    
    for (j=0;j<2;j++)
	{
	  trans[i][j]=B[j][i];
	  printf("\t%d",trans[i][j]);
	}
      printf("\n");
  }
}
