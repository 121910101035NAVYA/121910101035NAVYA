{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "name": "MID 1 CSD 121910101020.ipynb",
      "provenance": [],
      "collapsed_sections": []
    },
    "kernelspec": {
      "name": "python3",
      "display_name": "Python 3"
    },
    "language_info": {
      "name": "python"
    }
  },
  "cells": [
    {
      "cell_type": "code",
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "SJeZzxHyL_Q1",
        "outputId": "9f0452fd-075f-4bd1-ad69-b732132d6563"
      },
      "source": [
        "def ncr(n, r):\n",
        "    return (fact(n) / (fact(r)* fact(n - r)))\n",
        "def fact(n):\n",
        "    x = 1\n",
        "    for i in range(2, n+1):\n",
        "        x *= i\n",
        "    return x\n",
        "    \n",
        "    \n",
        "N = int(input(\"Enter Screws: \"))\n",
        "K = int(input(\"Enter K: \"))\n",
        "ans = (ncr(K,0)*ncr(N-K,2))/(ncr(N, 2))\n",
        "print('{0:.2g}'.format(ans))"
      ],
      "execution_count": 2,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Enter Screws: 10\n",
            "Enter K: 3\n",
            "0.47\n"
          ]
        }
      ]
    }

