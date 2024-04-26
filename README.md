# Python---8

{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "provenance": [],
      "authorship_tag": "ABX9TyNW2ji6b1XmydlYPucZ/Bjd",
      "include_colab_link": true
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
      "cell_type": "markdown",
      "metadata": {
        "id": "view-in-github",
        "colab_type": "text"
      },
      "source": [
        "<a href=\"https://colab.research.google.com/github/ciellleen/copyright/blob/main/8%EC%9D%BC%EC%B0%A8\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
      ]
    },
    {
      "cell_type": "code",
      "execution_count": null,
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "SZw7NOdvet9j",
        "outputId": "6d6a9ab9-f536-434b-dd98-6a689c4797ff"
      },
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "True\n",
            "True\n",
            "False\n",
            "False\n",
            "True\n",
            "True\n"
          ]
        }
      ],
      "source": [
        "text1 = \"네이스123\"\n",
        "text2 = \"1231231\"\n",
        "text3 = \"!@#\"\n",
        "text4 = \"!#1234\"\n",
        "text5 = \"nice\"\n",
        "text6 = \"nicew1234\"\n",
        "print(text1.isalnum())\n",
        "print(text2.isalnum())\n",
        "print(text3.isalnum())\n",
        "print(text4.isalnum())\n",
        "print(text5.isalnum())\n",
        "print(text6.isalnum())"
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "text = \"!#@#!@$!!@%@%!@@$231@3131이!!#@!네!@스$\"\n",
        "text1 = \"네이스\"\n",
        "text2 = \"123123\"\n",
        "text3 = \"!@#!\"\n",
        "check = \"\"\n",
        "print(text1.isalpha())\n",
        "print(text2.isalpha())\n",
        "print(text3.isalpha())\n",
        "for i in text:\n",
        "    if i.isalpha():\n",
        "        check += i\n",
        "print(check)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "_8FvS1epexE_",
        "outputId": "c494aa19-c937-4077-e230-dfe4476437c3"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "True\n",
            "False\n",
            "False\n",
            "이네스\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "a = \"BlockDMask\"\n",
        "b = \"1234Blog\"\n",
        "c = \"1231231\"\n",
        "d = \"-234\"\n",
        "e = \"1.23\"\n",
        "f = \"3\"\n",
        "g = '2/3'\n",
        "h = \"0\"\n",
        "print(f\"'{a}' .isdigit() : {str.isdigit(a)}\")\n",
        "print(f\"'{b}' .isdigit() : {str.isdigit(b)}\")\n",
        "print(f\"'{c}' .isdigit() : {str.isdigit(c)}\")\n",
        "print(f\"'{d}' .isdigit() : {str.isdigit(d)}\")\n",
        "print(f\"'{e}' .isdigit() : {str.isdigit(e)}\")\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "CNPX_0LrexHz",
        "outputId": "3e4debb0-41a3-4e23-b07d-f2a9c961fff3"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "'BlockDMask' .isdigit() : False\n",
            "'1234Blog' .isdigit() : False\n",
            "'1231231' .isdigit() : True\n",
            "'-234' .isdigit() : False\n",
            "'1.23' .isdigit() : False\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "a = '123456789'\n",
        "print(a.isdigit())\n",
        "print(a.isdecimal())\n",
        "print(a.isnumeric())\n",
        "print('\\n\\n')\n",
        "x ='3'\n",
        "print(x)\n",
        "print(x.isdigit())\n",
        "# True\n",
        "print(x.isdecimal())\n",
        "# False\n",
        "print(x.isnumeric())"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "Dk5A03H6exKz",
        "outputId": "168e073f-84d8-4d79-9bc2-0603d03004fd"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "True\n",
            "True\n",
            "True\n",
            "\n",
            "\n",
            "\n",
            "3\n",
            "True\n",
            "True\n",
            "True\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "a = \"I Love Python\"\n",
        "\n",
        "print(a.islower())\n",
        "print(a.islower())\n",
        "print(a.upper())\n",
        "print(a.lower())\n",
        "\n",
        "print('\\n\\n')\n",
        "\n",
        "str = \"This is string example...wow!!!\"\n",
        "print(str.islower())\n",
        "print(str.upper())\n",
        "\n",
        "str = \"this is string example...wow!!!\"\n",
        "print(str.islower())"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "hd6jzfCwexO_",
        "outputId": "0bf5cb4a-2633-4dab-de52-ee8a13b96748"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "False\n",
            "False\n",
            "I LOVE PYTHON\n",
            "i love python\n",
            "\n",
            "\n",
            "\n",
            "False\n",
            "THIS IS STRING EXAMPLE...WOW!!!\n",
            "True\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "str = \"This is string Example...Wow!!!\"\n",
        "print(str.swapcase())\n",
        "\n",
        "str = \"THIsis stRINg eXample...Wow!!!   1234\"\n",
        "print(str.swapcase())"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "qjgPXitjkkp6",
        "outputId": "f4c9b82b-29bc-4481-e109-9e9823f486a5"
      },
      "execution_count": 6,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "tHIS IS STRING eXAMPLE...wOW!!!\n",
            "thiSIS STrinG ExAMPLE...wOW!!!   1234\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "str = \"This Is String Example...Wow!!!\"\n",
        "print(str.istitle())\n",
        "\n",
        "str = \"This is string example...Wow!!!\"\n",
        "print(str.istitle())\n",
        "print(str.title())"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "EqV9pBhUkll4",
        "outputId": "6ec2e7c9-b1b5-4fd7-c8da-85a30d304bad"
      },
      "execution_count": 8,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "True\n",
            "False\n",
            "This Is String Example...Wow!!!\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "print('hello world!'.capitalize())\n",
        "print('HELLO WORLD!'.capitalize())"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "pFUFKinWkloe",
        "outputId": "40c978d5-db8d-4921-a279-46f5c41fb91c"
      },
      "execution_count": 7,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Hello world!\n",
            "Hello world!\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [],
      "metadata": {
        "id": "JdN5Sd6Gklqz"
      },
      "execution_count": null,
      "outputs": []
    }
  ]
}
